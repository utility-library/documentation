# SetGuardDifficulty
sets the difficulty of a guard 

| Argument     | Data Type | Needed                           | Default | Description                          |
|--------------|-----------|----------------------------------|---------|--------------------------------------|
| `guard`      | number    | :material-checkbox-blank-circle: | `-`     | The guard index                      |
| `difficulty` | string    | :material-checkbox-blank-circle: | `-`     | Can be: easy, medium, hard, veryhard |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetGuardDifficulty(guard, "medium")
    ```