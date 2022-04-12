# SetMarkerDrawOnEntity
Set the DrawOnEntity of the marker by the id

| Argument              | Data type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `DrawOnEntity`                | boolean | :material-checkbox-blank-circle: | `-` | The marker DrawOnEntity
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerDrawOnEntity("marker", true)
    ```