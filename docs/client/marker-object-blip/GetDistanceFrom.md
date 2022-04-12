# GetDistanceFrom
Get distance from a id

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Type`                | string | :material-checkbox-blank-circle: | `-` | The type of the id:<br><br> Marker, marker, m <br>`or`<br> Object, object, o
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | number | The distance of the marker or of the iObject

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    GetDistanceFrom("marker", "myid")
    ```