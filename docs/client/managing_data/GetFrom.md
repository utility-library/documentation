# GetFrom
Allows you to get the data saved through the [SetFor](http://127.0.0.1:8000/md/client/6_set_data/SetFor/)

| Argument              | Data Type                            | Nedeed                    | Default         | Description
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