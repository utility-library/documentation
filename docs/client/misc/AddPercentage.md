# AddPercentage
Add a percentage to a number.

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Number`                | number | :material-checkbox-blank-circle: | `-` | The number to add the percentage to
| `Percentage`            | number | :material-checkbox-blank-circle: | `-` | The percentage to add

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local p = AddPercentage(10, 20)
    local p2 = AddPercentage(40, 20)

    print(p, p2)
    ```

    ???+ success "Expected result"
        ```
        12, 48
        ```