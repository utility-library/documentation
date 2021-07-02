# SetMarkerRotation
Set the rotation of the marker by the id

| Argument              | Data type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Rotation`                | vector3 | :material-checkbox-blank-circle: | `-` | The marker rotation
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerRotation("marker", vector3(0.0, 1.0, 0.0))
    ```