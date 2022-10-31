# DisableControlAction
Disable a key, need to be called every tick

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Control`                | string | :material-checkbox-blank-circle: | `-` | The key to disable
| `Disable`                | boolean | :material-checkbox-blank-circle-outline: | `true` | Disable or no

!!! danger ""
    Need to be called every frame
---
??? example
    ```
    CreateLoop(function()
        DisableControlAction("K")
    end)
    ```
??? abstract "Old method"
    ```
    Citizen.CreateThread(function()
        while true do
            DisableControlAction(0, 311, true)
            Citizen.Wait(1)
        end
    end)
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_DisableControlAction`