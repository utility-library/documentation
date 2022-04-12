# DoesExist
Check if a marker/object exist

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the id:<br><br> Marker, marker, m <br>`or`<br> Object, object, o
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | boolean | True if exist, false if not exist

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    DoesExist("marker", "myid")
    ```