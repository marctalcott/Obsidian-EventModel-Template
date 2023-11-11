

<%* 
  let project = "Project";
  let destFolder = "";
  let agg = "";
  let date = tp.file.creation_date("YYYY-MM-DD");
  let title = tp.file.title;
  if (title.startsWith("Untitled")) {
    slice = await tp.system.prompt("Slice Name");
    agg = await tp.system.prompt("Aggregate Name");
    title = `${slice}-slice`
    await tp.file.rename(`${date}-${title}`);
    destFolder = `${project}/Slices`;
    await tp.file.move(`/${destFolder}/${slice}`);


}

%>

```yaml
status: New
user-story: 
dev: 
points: 
aggregate: <% agg %>

story: > As a user
I want to 
so that

Note: > 
```
#### Agg
[[<% agg %>]]

#### WFEs (0-many) 

#### APIs (0-many)

#### Command (1)

#### Events (1 to many)

#### Views (0 to many)


## AC

```yaml
G:  I am authorized
A:
W: 
T:

```
 
 