# RemovePercentage
Remove a percentage to a number.

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Number`                | number | :material-checkbox-blank-circle: | `-` | The number to remove the percentage to
| `Percentage`            | number | :material-checkbox-blank-circle: | `-` | The percentage to remove

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local p = RemovePercentage(10, 20)
    local p2 = RemovePercentage(40, 20)

    print(p, p2)
    ```

    ???+ success "Expected result"
        ```
        8, 32
        ```