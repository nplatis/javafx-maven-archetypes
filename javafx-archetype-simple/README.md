# Simple JavaFX Maven Archetype

The project is a Maven archetype for creating a simple JavaFX application.

### Prerequisites

* JDK 23
* Maven 3

### Create a project from a local repository

Once you have installed the archetype locally, you can use it to create a new project using:

```
mvn archetype:generate \
        -DarchetypeGroupId=nplatis \
        -DarchetypeArtifactId=javafx-archetype-simple \
        -DarchetypeVersion=25 \
        -Djavafx-version=25.0.2 \
        -DgroupId=groupid \
        -DartifactId=artifactId \
        -Dversion=version
```

The following properties can be customized while creating the project:

| Property                    | Default Value |
| --------------------------- | ------------- |
| javafx-version              | 25            |
| javafx-maven-plugin-version | 0.0.8         |
| add-debug-configuration     | N             |

For example:

```
mvn archetype:generate \
        -DarchetypeGroupId=nplatis \
        -DarchetypeArtifactId=javafx-archetype-fxml \
        -DarchetypeVersion=25 \
        -Djavafx-version=25.0.2 \
        -DgroupId=groupid \
        -DartifactId=artifactId \
        -Dversion=version \
        -Dadd-debug-configuration=Y
```
