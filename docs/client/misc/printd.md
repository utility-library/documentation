# printd
Dump a table, simply convert a table to a string

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table to dump
| `Advanced`                | boolean | :material-checkbox-blank-circle-outline: | `false` | Is true return an advanced dump of the table

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | string | The dumped table

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local _table = {
        message = "Hello"
    }

    printd(_table)
    ```
    ???+ success "Expected Results"
        ```
        {
            "message": "Hello"
        }
        ```