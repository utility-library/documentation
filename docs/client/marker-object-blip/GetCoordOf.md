# GetCoordOf
Get the coord from a id, return a vector3

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the id:<br><br> Marker, marker, m <br>`or`<br> Object, object, o
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | vector3 | The coords of the marker or of the iObject

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    GetCoordOf("marker", "myid")
    ```