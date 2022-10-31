# FindInTable
Return the index of the first row in the table that matches the given criteria.

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table to search.
| `Text`                | string | :material-checkbox-blank-circle: | `-` | The text to search for.

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local table = {
        "Jhon",
        "Doe",
        "Smith",
        "Robinson",
        "Smith",
        "George"
    }

    local i = FindInTable(table, "Smith")

    print(i)
    ```

    ???+ success "Expected result"
        ```
        3
        ```