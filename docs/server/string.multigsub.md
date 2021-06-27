# string.multigsub
Replace multiple part of a string

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `String`                | string | :material-checkbox-blank-circle: | `-` | The original texture
| `Pattern`                | table | :material-checkbox-blank-circle: | `-` | The pattern to find and replace
| `Replacement`                | table | :material-checkbox-blank-circle: | `-` | The replacemente table

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local string = "i love me"

    local new_string = string.multigsub(string, {"love", "me"}, {"hate", "you"})

    print(new_string)
    ```

    ???+ success "Expected result"
        `i hate you`