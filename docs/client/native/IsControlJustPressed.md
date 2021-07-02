# IsControlJustPressed
Call a callback when a specific key was pressed, more optimized and easy to use

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Control`                | string | :material-checkbox-blank-circle: | `-` | The key, [this is the list](https://docs.fivem.net/docs/game-references/input-mapper-parameter-ids/keyboard/)
| `Callback`                | function | :material-checkbox-blank-circle: | `-` | The code executed when the key was pressed

!!! success ""
    Dont need to be called every frame

---
??? example
    Run at **0** ms
    ```
    IsControlJustPressed("K", function()
        print("Hello")
    end)
    ```
??? abstract "Old method"
    Run at **2/3** ms
    ```
    Citizen.CreateThread(function()
        while true do
            if IsControlJustPressed(0, 311) then
                print("Hello")
            end
            Citizen.Wait(1)
        end
    end)
    ```
    ??? info "IsControlJustPressed"
        although i dont recommend it, you can use the old native via `old_IsControlJustPressed`