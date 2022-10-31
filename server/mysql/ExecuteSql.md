# ExecuteSql
Execute any type of sql query, automatically detect the query

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Query`                | string | :material-checkbox-blank-circle: | `-` | The query
| `Params`                | table | :material-checkbox-blank-circle: | `-` | The query params

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    ExecuteSql("INSERT INTO utility_db_integration SET data = @data", {
        ["@data"] = "Hello"
    })

    local data = ExecuteSql("SELECT * FROM utility_db_integration")
    ```