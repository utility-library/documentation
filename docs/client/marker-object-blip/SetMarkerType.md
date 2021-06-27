# SetMarkerType
Set the type of the marker by the id

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Type`                | number | :material-checkbox-blank-circle: | `-` | The [marker type](https://docs.fivem.net/docs/game-references/markers/)
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerType("marker", 2)
    ```