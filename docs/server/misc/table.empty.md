# table.empty
Check if a table is empty

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | True if is empty, false if have some data
    

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local emptytable = {}

    print(table.empty(emptytable))
    ```

    ???+ success "Expected result"
        `true`
