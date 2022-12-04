<<<<<<< HEAD
# GetDataForJob
Return the number of player that have that job and the workers list of that job

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Job`                | string | :material-checkbox-blank-circle: | `-` | The job name

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The number of player with that job
    | table | A table with all the id of the players with that job

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local count, workers = GetDataForJob("police")
    
    -- count = 3
    -- workers = {3, 5, 19} 
    ```     
=======
# GetDataForJob
Return the number of player that have that job and the workers list of that job

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Job`                | string | :material-checkbox-blank-circle: | `-` | The job name

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The number of player with that job
    | table | A table with all the id of the players with that job

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local count, workers = GetDataForJob("police")
    
    -- count = 3
    -- workers = {3, 5, 19} 
    ```     
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
