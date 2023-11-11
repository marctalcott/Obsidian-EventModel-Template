
<%* 
  let project = "Project";
  let destFolder = "";
  let agg = "";
  let date = tp.file.creation_date("YYYY-MM-DD");
  let title = tp.file.title;
  if (title.startsWith("Untitled")) {
    api = await tp.system.prompt("API Name");

    title = `${api}-api`
    destFolder = `${project}/API`;
    await tp.file.move(`/${destFolder}/${title}`);
}

%>

```yaml
api: <%api%>
   verb:
   url:
   body:
     f:
	    - Id


note: ""

```