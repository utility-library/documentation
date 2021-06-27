# CreateObject
Is equal to the standard one but dont need to load or request the model

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `ModelHash`                | string/hash | :material-checkbox-blank-circle: | `-` | The hash or the name of the model
| `Coords`                | vector3/number | :material-checkbox-blank-circle: | `-` | The coordinates to create the object (can be an vector3 or you can insert it one by one)
| `IsNetwork`                | boolean | :material-checkbox-blank-circle-outline: | `false` | Whether to create a network object for the object. If false, the object exists only locally.
| `NetMissionEntity`         | boolean | :material-checkbox-blank-circle-outline: | `false` | Whether to register the object as pinned to the script host in the R* network model.
| `DoorFlag`         | boolean | :material-checkbox-blank-circle-outline: | `false` | False to create a door archetype (archetype flag bit 26 set) as a door. Required to be set to true to create door models in network mode.

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | object | A script handle (fwScriptGuid index) for the object, or 0 if the object failed to be created
    | netId | The net id
    
!!! success ""
    Dont need to be called every frame
---
??? example
    Using **vector3**
    ```
    local obj, netId = CreateObject("prop_weed_01", vector3(0.0, 0.0, 0.0), true, false, false)
    ```
    Using **separated coords**
    ```
    local obj, netId = CreateObject("prop_weed_01", 0.0, 0.0, 0.0, true, false, false)
    ```
??? abstract "Old method"
    ```
    local modelHash = GetHashKey("prop_weed_01")

    if not HasModelLoaded(modelHash) then
        RequestModel(modelHash);
        while not HasModelLoaded(modelHash) do 
            Citizen.Wait(1); 
        end  
    end
    
    local obj = CreateObject(modelHash, 0.0, 0.0, 0.0, true, false, false)
    SetModelAsNoLongerNeeded(modelHash) 
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_CreateObject`