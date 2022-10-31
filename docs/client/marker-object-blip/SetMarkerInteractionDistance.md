# SetMarkerInteractionDistance
Set the interaction distance of the marker by the id

| Argument              | Data type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `distance`                | number | :material-checkbox-blank-circle: | `-` | The new marker interaction distance
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerInteractionDistance("marker", 4.0)
    ```