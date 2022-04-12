# table.clone
Clone a table

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The original table

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | table | The cloned table

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local tabletoclone = {
        msg = "Hello"
    }

    local cloned_table = table.clone(tabletoclone)

    print(cloned_table.msg)
    ```

    ???+ success "Expected result"
        `Hello`
