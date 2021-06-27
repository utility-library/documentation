# SetMarkerDirection
Set the direction of the marker by the id

| Argument              | Data type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Direction`                | vector3 | :material-checkbox-blank-circle: | `-` | The marker direction
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerDirection("marker", vector3(0.0, 0.0, 0.0))
    ```