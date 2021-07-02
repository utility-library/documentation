# SetMarkerColor
Set the color of the marker by the id

| Argument              | Data type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Color`                | vector3 | :material-checkbox-blank-circle: | `-` | The marker color (RGB)
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerColor("marker", {255, 0, 255})
    ```