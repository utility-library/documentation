# _g
Register a global variable on all scripts that load the Utility

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Name`                | string | :material-checkbox-blank-circle: | `-` | The name of the variable
| `Value`                | any | :material-checkbox-blank-circle: | `-` | The value of the variable

!!! warning
    Any other resource where you want to use the global variable must be started **BEFORE** the resource where you define the variable

!!! success ""
    Dont need to be called every frame
---
??? example
    I create the global on the script `this_is_a_test`
    ```
    _g("utility", "Utility is amazing!")
    ```

    If I go in another script that has the Utility loaded and printout the variable `utility` it will write "Utility is amazing!".
    ???+ success "Expected result"
        Resource "this_is_a_test":
        ```
        print(utility)
        ```
        Return `Utility is amazing!`

        ---

        Resource "this_is_another_resource":
        ```
        print(utility)
        ```
        Return `Utility is amazing!`