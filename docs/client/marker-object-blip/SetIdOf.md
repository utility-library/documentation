# SetIdOf
Change the id of a marker/iObject by the id

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the id:<br><br> Marker, marker, m <br>`or`<br> Object, object, o
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The old id
| `New id`                | string/number | :material-checkbox-blank-circle: | `-` | The new id

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetIdOf("marker", "myid", "newid")
    ```