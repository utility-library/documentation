# SetPedStatic
Freeze the ped, make it ignore any event (ex. shooting) and puts it invincible

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `ped`                | entity | :material-checkbox-blank-circle: | `-` | The ped that need to be modified
| `active`                | boolean | :material-checkbox-blank-circle: | `-` | If active or no


!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetPedStatic(ped, true)
    ```
??? abstract "Old method"
    ```
    FreezeEntityPosition(ped, true)
    SetEntityInvincible(ped, true)
    SetBlockingOfNonTemporaryEvents(ped, true)
    ```