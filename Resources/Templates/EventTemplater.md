
<%* 
  let project = "Project";
  let destFolder = "";
  let agg = "";
  let date = tp.file.creation_date("YYYY-MM-DD");
  let title = tp.file.title;
  if (title.startsWith("Untitled")) {
    event = await tp.system.prompt("Event Name");

    title = `${event}-event`
    destFolder = `${project}/Events`;
    await tp.file.move(`/${destFolder}/${title}`);
}

%>

```yaml
cmd: <%event%>
	- Id


note: ""

```