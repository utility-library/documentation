# GetRandom
Return a random value from the given table, use indexes to random the value.

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table to get a random index from

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

    local r = GetRandom(table)
    local r2 = GetRandom(table)

    print(r, r2)
    ```

    ???+ success "Expected result"
        ```
        Smith,  George
        ```