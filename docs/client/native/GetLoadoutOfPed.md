# GetLoadoutOfPed
Returns the ped weapons loadout

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Ped`                | ped | :material-checkbox-blank-circle-outline: | `` | The ped

??? success "Returns"
    | Child     | Data Type | Description                           |
    |-----------|-----------|---------------------------------------|
    | name      | string    | Weapon model name                            |
    | hash      | number    | Hash of the weapon                         |
    | ammo     | number     | Weapon ammo                           |
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local loadout = GetLoadoutOfPed(ped)

    for i=1, #loadout do
        print("Weapon model = "..loadout[i].name.." Weapon Hash = "..loadout[i].hash.." Weapon Ammo = "..loadout[i].ammo)
    end
    ```