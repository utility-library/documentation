# GetDataFromDb
Allows you to get data from the *utility_db_integration* table

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
        `* = select all`

        Get some data from the db using some where parameter (**single**)
        ```
        GetDataFromDb("SELECT * WHERE id = 1")
        ```

        Get some data from the db using some where parameter (**multi**)
        ```
        GetDataFromDb("SELECT data2 WHERE id, data = 1, example")
        ```
    ??? info "Without the where"
        `* = select all`

        Get some data from the db (**single**)
        ```
        GetDataFromDb("SELECT *")
        ```
        ---
        Get some data from the db (**multi**)
        ```
        GetDataFromDb("SELECT data, data2")
        ```
    ???+ warning
        If you want to use multi table you need to create the table by yourself