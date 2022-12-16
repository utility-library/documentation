# BreakDoorWithThermalCharge
Plays the thermal charge scene on the given door, automatically finds all the data it needs, and moves the player to the start coordinates

| Argument       | Data Type | Needed                                   | Default | Description                                                                                  |
|----------------|-----------|------------------------------------------|---------|----------------------------------------------------------------------------------------------|
| `door`         | object    | :material-checkbox-blank-circle:         | `-`     |                                                                                              |
| `bagComponent` | number    | :material-checkbox-blank-circle-outline: | `45`    | Of note that the native replaces the bag, you will have to give him the player's initial bag |
| `duration`     | number    | :material-checkbox-blank-circle-outline: | `3000`  | Total duration of lock stripping in ms                                                       |

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local coords = GetEntityCoords(PlayerPedId())
    local door = GetClosestObjectOfType(coords, 4.0, `hei_v_ilev_bk_gate_pris`)

    if door > 0 then
        BreakDoorWithThermalCharge(door)
    end
    ```