
<%* 
  let project = "Project";
  let destFolder = "";
  let agg = "";
  let date = tp.file.creation_date("YYYY-MM-DD");
  let title = tp.file.title;
  if (title.startsWith("Untitled")) {
    wfe = await tp.system.prompt("WFE Name");

    title = `${wfe}-wfe`
    destFolder = `${project}/WFE`;
    await tp.file.move(`/${destFolder}/${title}`);
}

%>

```yaml
wfe: <%wfe%>
	handler:
	   handles:
	   logic: >
	   


note: ""

```