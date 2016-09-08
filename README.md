# ETS4Reader

ETS4 Project Reader ...

Reads .knxproj files and provides  the gathered information in an object hierarchie.

```
File file = new File("myknxproject.knxproj");
KnxProjReader kpr = new KnxProjReader(file);
List<GroupAddress> groupaddressList = kpr.getProjects().get(0).getGroupaddressList();
```
See javadoc of Project, GroupAddress and Device for more details.

## How to install and run on OS X
`brew install maven`

`mvn install`

```
java -cp target/ets4reader-1.0.0-SNAPSHOT.jar de.root1.ets4reader.ETS4Reader /PATH/TO/.knxproj
```
