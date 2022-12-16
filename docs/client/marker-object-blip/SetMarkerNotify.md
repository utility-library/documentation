# SetMarkerNotify [New]
Set the notify of the marker by the id

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to update the marker
| `Notify`                | string | :material-checkbox-blank-circle: | `-` | The ButtonNotification data
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetMarkerNotify("marker", "Press [E] to interact")
    ```