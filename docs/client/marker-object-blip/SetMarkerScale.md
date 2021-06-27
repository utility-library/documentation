# SetMarkerScale
Set the scale of the marker by the id

| Argument              | Data type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Scale`                | vector3 | :material-checkbox-blank-circle: | `-` | The marker scale
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerscale("marker", vector3(1.0, 1.0, 1.5))
    ```