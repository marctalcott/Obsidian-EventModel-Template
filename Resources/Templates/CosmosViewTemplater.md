
<%* 
  let project = "Project";
  let destFolder = "";
  let agg = "";
  let date = tp.file.creation_date("YYYY-MM-DD");
  let title = tp.file.title;
  if (title.startsWith("Untitled")) {
    view = await tp.system.prompt("View Name");

    title = `${view}-view`
    destFolder = `${project}/Views-Cosmos`;
    await tp.file.move(`/${destFolder}/${title}`);
}

%>
## Cosmos View

```yaml
cmd: <%view%>
	- Id


note: ""

```