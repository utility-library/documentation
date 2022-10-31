# SetGuardRoute
sets the route of a guard 

| Argument | Data Type | Needed                           | Default | Description       |
|----------|-----------|----------------------------------|---------|-------------------|
| `guard`  | number    | :material-checkbox-blank-circle: | `-`     | The guard index   |
| `route`  | route     | :material-checkbox-blank-circle: | `-`     | The route id/name |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetGuardRoute(guard, "test")
    ```