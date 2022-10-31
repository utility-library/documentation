# AddPlayerToScene
Add a player to an existing scene

| Argument          | Data Type | Needed                                   | Default | Description                          |
|-------------------|-----------|------------------------------------------|---------|--------------------------------------|
| `player`          | player    | :material-checkbox-blank-circle:         | `-`     | The player client id (PlayerId)      |
| `scene`           | scene     | :material-checkbox-blank-circle:         | `-`     | The scene netid                      |
| `dict`            | string    | :material-checkbox-blank-circle:         | `-`     | The anim dict that the ped will play |
| `name`            | string    | :material-checkbox-blank-circle:         | `-`     | The anim name that the ped will play |
| `speed`           | number    | :material-checkbox-blank-circle-outline: | `4.0`   |                                      |
| `speedMultiplier` | number    | :material-checkbox-blank-circle-outline: | `-8.0`  |                                      |
| `flag`            | number    | :material-checkbox-blank-circle-outline: | `1`     |                                      |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    AddPlayerToScene(PlayerId(), scene, "somedict", "somename")
    ```