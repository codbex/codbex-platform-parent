# codbex-platform-parent
Parent Module for Platform Products

## Pom properties

| Property Name  | Description                      | Default Value |
|--|--|--|
| skip.unit.tests | Skips unit tests (*.Test)        | false |
| skip.integration.tests | Skips integration tests  (*.IT)  | true |
| skip.code.formatting | Skips java code formatting       | false |
| maven.javadoc.skip | Skips javadoc                    | false |
| license.skip | Skips license headers generation | false |

## Profiles

| Profile Name           | Description                                                                       |
|------------------------|-----------------------------------------------------------------------------------|
| tests        | Run unit and integration tests                                                    |
| unit-tests | Run unit tests                                                                    |
| integration-tests | Run integration tests                                                             |
| quick-build     | Build project skipping tests, javadoc, licensing and code formatting |

To activate a profile, add it to the maven command.<br>Example:
```
    mvn clean install -P quick-build
```
