# TaskPlayAnim
Is equal to the standard one but dont need to load or request the anim dict

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Ped`                | ped | :material-checkbox-blank-circle: | `-` | The ped
| `Animation dictionary` | string | :material-checkbox-blank-circle: | `-` | The animation dictionary, [this is the list](https://alexguirre.github.io/animations-list/)
| `Animation name`       | string | :material-checkbox-blank-circle: | `-` | The animation name, [this is the list](https://alexguirre.github.io/animations-list/)
| `Blend in speed`       | number | :material-checkbox-blank-circle: | `-` | The blend in speed
| `Blend out speed`      | number | :material-checkbox-blank-circle: | `-` | The blend out speed
| `Duration`             | number | :material-checkbox-blank-circle: | `-` | The duration time in milliseconds (**ms**)
| `Flag`                 | number | :material-checkbox-blank-circle: | `-` | The animation flag: -1 default. 0 no play, small value = slow animation speed, other = freeze player
| `Playback Rate`        | number | :material-checkbox-blank-circle: | `-` | No description, values are between 0.0 and 1.0  
| `LockX`                | boolean | :material-checkbox-blank-circle-outline: | `0` | No description, 0 in most cases
| `LockY`                | boolean | :material-checkbox-blank-circle-outline: | `0` | No description, 0 in most cases
| `LockZ`                | boolean | :material-checkbox-blank-circle-outline: | `0` | No description, 0 in most cases

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    TaskPlayAnim(PlayerPedId(), "amb@world_human_golf_player@male@idle_a", "idle_a", 8.0, 1.0, -1, 49, 0)
    ```
??? abstract "Old method"
    ```
    if not HasAnimDictLoaded("amb@world_human_golf_player@male@idle_a") then
        RequestAnimDict("amb@world_human_golf_player@male@idle_a")
        while not HasAnimDictLoaded("amb@world_human_golf_player@male@idle_a") do 
            Citizen.Wait(1) 
        end
    end

    TaskPlayAnim(PlayerPedId(), "amb@world_human_golf_player@male@idle_a", "idle_a", 8.0, 1.0, -1, 49, 0)
    RemoveAnimDict("amb@world_human_golf_player@male@idle_a")
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_TaskPlayAnim`