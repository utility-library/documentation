# CreateVehicle
Is equal to the standard one but dont need to load or request the model

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `ModelHash`                | string/hash | :material-checkbox-blank-circle: | `-` | The hash or the name of the model
| `Coords`                | vector3/number | :material-checkbox-blank-circle: | `-` | The coordinates to create the object (can be an vector3 or you can insert it one by one)
| `Heading`                | number | :material-checkbox-blank-circle: | `0` | Heading to face towards, in degrees.
| `IsNetwork`                | boolean | :material-checkbox-blank-circle-outline: | `false` | Whether to create a network object for the vehicle. If false, the vehicle exists only locally.
| `NetMissionEntity`         | boolean | :material-checkbox-blank-circle-outline: | `false` | Whether to register the vehicle as pinned to the script host in the R* network model.

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | vehicle | A script handle (fwScriptGuid index) for the vehicle, or 0 if the vehicle failed to be created
    | netId | The net id
!!! success ""
    Dont need to be called every frame
---
??? example
    Using **vector3**
    ```
    local veh, netId = CreateVehicle("t20", vector3(0.0, 0.0, 0.0), 0.0, true, false)
    ```
    Using **separated coords**
    ```
    local veh, netId = CreateVehicle("t20", 0.0, 0.0, 0.0, 0.0, true, false)
    ```
??? abstract "Old method"
    ```
    local modelHash = GetHashKey("t20")

    if not HasModelLoaded(modelHash) then
        RequestModel(modelHash);
        while not HasModelLoaded(modelHash) do 
            Citizen.Wait(1); 
        end  
    end
    
    local obj = CreateVehicle(modelHash, 0.0, 0.0, 0.0, 0.0, true, false)
    SetModelAsNoLongerNeeded(modelHash) 
    ```
    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_CreateVehicle`