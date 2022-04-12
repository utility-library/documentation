# SetMarkerCoords
Set the coords of the marker by the id

| Argument              | Data type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The marker coords
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerCoords("marker", vector3(0.0, 0.0, 0.0))
    ```