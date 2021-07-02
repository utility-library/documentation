# table.remove
Equal to the native table.remove of lua but accept string as position

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Table`                | table | :material-checkbox-blank-circle: | `-` | The table
| `Position`                | number/string | :material-checkbox-blank-circle: | `-` | The position of the data to remove

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local tabletocheck = {
        ["Hello"] = 5,
        ["Utility"] = 1,
    }

    table.remove(tabletocheck, "Hello")

    print(json.encode(tabletocheck))
    ```

    ???+ success "Expected result"
        `{"Utility":1}`