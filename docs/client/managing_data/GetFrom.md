# GetFrom
Allows you to get the data saved through the [SetFor](https://utility-library.github.io/client/managing_data/SetFor/)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id
| `Property`                | string/table | :material-checkbox-blank-circle-outline: | `-` | The data name


!!! success ""
    Dont need to be called every frame
---
??? example
    Get a **specific** data saved for that property
    ```
    GetFrom("myid", "something")  
    ```
    Return `"Hello"` (string)

    ---

    Get **all** data saved for that property
    ```
    GetFrom("myid")         
    ```
    Return `{ something = "Hello", something2 = 5, something3 = {1, 2, 3} }` (table)