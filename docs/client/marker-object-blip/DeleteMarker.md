# DeleteMarker
Delete a marker by the id

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Id`                | string/number | :material-checkbox-blank-circle: | `-` | The id to delete the marker
    
!!! success ""
    Dont need to be called every frame, if called every frame and the marker dont exist, sleep the loop for 100 ms to prevent spam
---
??? example
    ```
    DeleteMarker("marker")
    ```