# CreatePed
Is equal to the standard one but dont need to load or request the model

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Model`                | string/number | :material-checkbox-blank-circle: | `-` | The hash or the name of the model
| `Coords`                | vector3/number | :material-checkbox-blank-circle: | `-` | The coordinates to create the ped (can be an vector3 or you can insert it one by one)
| `Heading`                | number | :material-checkbox-blank-circle: | `-` | The heading to create the ped
| `IsNetwork`                | boolean | :material-checkbox-blank-circle: | `-` | Whether to create a network object for the ped. If false, the ped exists only locally.

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | ped | A script handle (fwScriptGuid index) for the ped, or 0 if the ped failed to be created.
    | netId | The net id
    
!!! success ""
    Dont need to be called every frame
---
??? example
    Using **vector3**
    ```
    local ped, netId = CreatePed("cs_dale", vector3(0.0, 0.0, 0.0), 5.0, true)
    ```
    Using **separated coords**
    ```
    local ped, netId = CreatePed("cs_dale", 0.0, 0.0, 0.0, 5.0, true)
    ```
??? abstract "Old method"
    ```
    local modelHash = GetHashKey("cs_dale")

    if not HasModelLoaded(modelHash) then
        RequestModel(modelHash);
        while not HasModelLoaded(modelHash) do 
            Citizen.Wait(1); 
        end  
    end
    
    local ped = CreatePed(0, modelHash, 0.0, 0.0, 0.0, 5.0, true, false)
    SetModelAsNoLongerNeeded(modelHash) 
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_CreatePed`