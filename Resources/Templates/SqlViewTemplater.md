
<%* 
  let project = "Project";
  let destFolder = "";
  let agg = "";
  let date = tp.file.creation_date("YYYY-MM-DD");
  let title = tp.file.title;
  if (title.startsWith("Untitled")) {
    view = await tp.system.prompt("View Name");

    title = `${view}-view`
    destFolder = `${project}/Views-Sql`;
    await tp.file.move(`/${destFolder}/${title}`);
}

%>
## SQL Table

```yaml
cmd: <%view%>
	- Id


note: ""

```