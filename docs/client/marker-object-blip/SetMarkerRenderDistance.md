# SetMarkerRenderDistance
Set the render distance of the marker by the id

| Argument              | Data type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `distance`                | number | :material-checkbox-blank-circle: | `-` | The new marker render distance
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerRenderDistance("marker", 4.0)
    ```