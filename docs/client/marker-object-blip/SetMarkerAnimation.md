# SetMarkerAnimation
Set the bouncing animation of the marker by the id

| Argument              | Data type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Animation`                | boolean | :material-checkbox-blank-circle: | `-` | Use or no the bouncing animation
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerAnimation("marker", true)
    ```