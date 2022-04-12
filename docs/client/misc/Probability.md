# Probability
Pick a random number between 0 and 100, and if is lower or equal than the given value, return true.

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Number`                | number | :material-checkbox-blank-circle: | `-` | The number to compare with

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local p = Probability(10)
    local p2 = Probability(100)

    print(p, p2)
    ```

    ???+ success "Expected result"
        ```
        false,  true
        ```