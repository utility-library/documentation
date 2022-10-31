# WaitNear
Wait that the player is near to a specific position, is sync, so it will wait all the code until the player is not near the position.

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coordinates to wait near
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    WaitNear(vector3(0.0, 0.0, 0.0))
    ```