# table.fexist
Check if the field exist in the table

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table
| `Field`                | string | :material-checkbox-blank-circle: | `-` | The field to check

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | True if field exist, false if field dont exist
    

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local tabletocheck = {
        msg = "Message",
        another = 2
    }

    print(table.fexist(tabletocheck, "msg"))
    print(table.fexist(tabletocheck, "utility"))
    ```

    ???+ success "Expected result"
        `true`<br>
        `false`