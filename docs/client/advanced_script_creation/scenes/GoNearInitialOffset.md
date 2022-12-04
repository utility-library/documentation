<<<<<<< HEAD
# GoNearInitialOffset
Moves the player to the starting offest (this should be perfect, its semi reversed from R* scripts)

| Argument | Data Type  | Needed                           | Default | Description                                                        |
|----------|------------|----------------------------------|---------|--------------------------------------------------------------------|
| `player` | player/ped | :material-checkbox-blank-circle: | `-`     | The player ped id (PlayerPedId) or the player client id (PlayerId) |
| `coords` | vector3    | :material-checkbox-blank-circle: | `-`     | Starting coords to calculate the animation offset                  |
| `rot`    | vector3    | :material-checkbox-blank-circle: | `-`     | Starting rotation to calculate the animation offset                |
| `dict`   | string     | :material-checkbox-blank-circle: | `-`     | The animation dict where to find the offset                        |
| `name`   | string     | :material-checkbox-blank-circle: | `-`     | The animation name where to find the offset                        |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local player = PlayerPedId()
    local coords = GetEntityCoords(player)
    local rot = GetEntityCoords(player)

    GoNearInitialOffset(player, coords, rot, "somedict", "somename")
=======
# GoNearInitialOffset
Moves the player to the starting offest (this should be perfect, its semi reversed from R* scripts)

| Argument | Data Type  | Needed                           | Default | Description                                                        |
|----------|------------|----------------------------------|---------|--------------------------------------------------------------------|
| `player` | player/ped | :material-checkbox-blank-circle: | `-`     | The player ped id (PlayerPedId) or the player client id (PlayerId) |
| `coords` | vector3    | :material-checkbox-blank-circle: | `-`     | Starting coords to calculate the animation offset                  |
| `rot`    | vector3    | :material-checkbox-blank-circle: | `-`     | Starting rotation to calculate the animation offset                |
| `dict`   | string     | :material-checkbox-blank-circle: | `-`     | The animation dict where to find the offset                        |
| `name`   | string     | :material-checkbox-blank-circle: | `-`     | The animation name where to find the offset                        |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local player = PlayerPedId()
    local coords = GetEntityCoords(player)
    local rot = GetEntityCoords(player)

    GoNearInitialOffset(player, coords, rot, "somedict", "somename")
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
    ```