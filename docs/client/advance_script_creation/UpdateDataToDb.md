# UpdateDataToDb
Allows you to update data that already exist in the *utility_db_integration* table

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Options`                | string | :material-checkbox-blank-circle: | `-` | The options, see below for more info, the logic its pretty equal to the `MySQL` query

???+ warning
    For server safety, the trigger below the function can be disabled in the utility config<br>
    if you want to use this native you need to execute the SQL

!!! success ""
    Dont need to be called every frame
---
??? example
    ??? info "With the where"
        Update some data that already exist in the db using some where parameter (**single**)
        ```
        UpdateDataToDb("UPDATE data = example WHERE id = 1")
        ```

        Update some data that already exist in the db using some where parameter (**multi**)
        ```
        UpdateDataToDb("UPDATE data, data2 = example, example2 WHERE id = 1")
        ```
    ??? info "Without the where"
        Update some data that already exist in the db (**single**)
        ```
        SaveDataToDb("UPDATE data = example")
        ```
        ![image](https://i.postimg.cc/L4yXMZLS/image.png)
        ---
        Update some data that already exist in the db (**multi**)
        ```
        SaveDataToDb("UPDATE data, data2 = example, example2")
        ```
        ![image](https://i.postimg.cc/6Q9J3Mxm/image.png)
    ???+ warning
        If you want to use multi table you need to create the table by yourself