<<<<<<< HEAD
# CreateGuard
Creates a guard that can be assigned a route

| Argument     | Data Type     | Needed                                   | Default | Description                                                       |
|--------------|---------------|------------------------------------------|---------|-------------------------------------------------------------------|
| `model`      | string/number | :material-checkbox-blank-circle:         | `-`     | The ped model                                                     |
| `coords`     | vector3       | :material-checkbox-blank-circle:         | `-`     |                                                                   |
| `heading`    | number        | :material-checkbox-blank-circle:         | `-`     |                                                                   |
| `difficulty` | string        | :material-checkbox-blank-circle-outline: | `-`     | Can be: easy, medium, hard, veryhard                              |
| `guardRoute` | route         | :material-checkbox-blank-circle-outline: | `-`     | The route id (created using [CreateGuardRoute](CreateGuardRoute)) |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | ped | The guard ped

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local guard = CreateGuard("mp_m_securoguard_01", vector3(241.67, 222.49, 106.29), 0.0, "easy")
    GiveWeaponToPed(guard, `WEAPON_PISTOL`, 255, false, true)

=======
# CreateGuard
Creates a guard that can be assigned a route

| Argument     | Data Type     | Needed                                   | Default | Description                                                       |
|--------------|---------------|------------------------------------------|---------|-------------------------------------------------------------------|
| `model`      | string/number | :material-checkbox-blank-circle:         | `-`     | The ped model                                                     |
| `coords`     | vector3       | :material-checkbox-blank-circle:         | `-`     |                                                                   |
| `heading`    | number        | :material-checkbox-blank-circle:         | `-`     |                                                                   |
| `difficulty` | string        | :material-checkbox-blank-circle-outline: | `-`     | Can be: easy, medium, hard, veryhard                              |
| `guardRoute` | route         | :material-checkbox-blank-circle-outline: | `-`     | The route id (created using [CreateGuardRoute](CreateGuardRoute)) |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | ped | The guard ped

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local guard = CreateGuard("mp_m_securoguard_01", vector3(241.67, 222.49, 106.29), 0.0, "easy")
    GiveWeaponToPed(guard, `WEAPON_PISTOL`, 255, false, true)

>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
    ```