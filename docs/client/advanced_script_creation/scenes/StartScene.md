# StartScene
Start an existing scene

| Argument              | Data Type | Needed                                   | Default | Description                                                                       |
|-----------------------|-----------|------------------------------------------|---------|-----------------------------------------------------------------------------------|
| `scene`               | string    | :material-checkbox-blank-circle:         | `-`     | The scene netid                                                                   |
| `goNearInitialOffset` | boolean   | :material-checkbox-blank-circle-outline: | `-`     | If true it will automatically move every player near the initial animation offset |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    StartScene(scene, true)
    ```