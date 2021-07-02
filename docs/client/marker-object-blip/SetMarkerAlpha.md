# SetMarkerAlpha
Set the alpha of the marker by the id

| Argument              | Data type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Alpha`                | number | :material-checkbox-blank-circle: | `-` | The marker alpha, from 0 to 255
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerAlpha("marker", 255)
    ```