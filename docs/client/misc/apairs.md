# apairs
Pairs a table in alphabetical order

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local table = {
        ["Z"] = true,
        ["B"] = true,
        ["A"] = true,
        ["G"] = true
    }
    

    for k,v in apairs(table) do
        print(k,v)
    end
    ```

    ???+ success "Expected result"
        ```
        A	true
        B	true
        G	true
        Z	true
        ```
