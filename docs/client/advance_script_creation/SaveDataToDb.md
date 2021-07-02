# SaveDataToDb
Allows you to save data in the *utility_db_integration* table

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Options`                | string | :material-checkbox-blank-circle: | `-` | The options, see below for more info

???+ warning
    For server safety, the trigger below the function can be disabled in the utility config<br>
    if you want to use this native you need to execute the SQL

!!! success ""
    Dont need to be called every frame
---
??? example
    Saving some data to the db (**single**)
    ```
    SaveDataToDb("INSERT data = example")
    ```
    ![image](https://i.postimg.cc/L4yXMZLS/image.png)
    ---
    Saving some data to the db (**multi**)
    ```
    SaveDataToDb("INSERT data, data2 = example, example2")
    ```
    ![image](https://i.postimg.cc/6Q9J3Mxm/image.png)
    ???+ warning
        If you want to use multi table you need to create the table by yourself