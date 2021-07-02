# SetFor
Allows you to manipulate a table already created by the utility without having to create it every time

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id
| `Property`                | string/table | :material-checkbox-blank-circle: | `-` | The data
| `Value`                | any | :material-checkbox-blank-circle-outline: | `-` | The value
| `Synced`                | boolean | :material-checkbox-blank-circle-outline: | `false` | Sync or the data for all script that load the utility


!!! success ""
    Dont need to be called every frame
---
??? example
    Here you can set any, i told ANY, value to an marker, an iObject, an number or anything else

    Set data one by one
    ```
    SetFor("myid", "something", "Hello")
    SetFor("myid", "something2", 5)
    SetFor("myid", "something3", {1, 2, 3})
    ```

    Set data with a table
    ```
    SetFor("myid", {
        something = "Hello"
        something2 = 5
        something3 = {1, 2, 3}
    })
    ```

    ??? info "Synced data"
        In the script "utility_test" if call the setfor with synced arguments to true
        ```
            SetFor("myid", "something", "Hello", true)

            --or

            SetFor("myid", {
                something = "Hello"
            }, true)
        ```

        Now i call the GetFrom from the resource "utility_test2" and the data will be synced
        ```
        GetFrom("myid", "something") 
        ```
        Return `Hello` (string)