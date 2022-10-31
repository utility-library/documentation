# CreateTrolly
Create a lootable trolly, everything will be handled automatically by the lib, you just have to give the money and define the type of trolly

| Argument   | Data Type | Needed                                   | Default                                 | Description                                                       |
|------------|-----------|------------------------------------------|-----------------------------------------|-------------------------------------------------------------------|
| `type`     | string    | :material-checkbox-blank-circle:         | `-`                                     | The type of trolly: cash, gold, diamond                           |
| `coords`   | vector3   | :material-checkbox-blank-circle:         | `-`                                     |                                                                   |
| `giveCash` | function  | :material-checkbox-blank-circle:         | `-`                                     | This function is executed each time a money bundle enters the bag |
| `notify`   | string    | :material-checkbox-blank-circle-outline: | `Press {E} to begin looting the trolly` | Marker notification to interact with the cart                     |
| `minSpeed` | number    | :material-checkbox-blank-circle-outline: | `1.0`                                   | minimum speed at which the player can loot (1.0 = normal speed)   |
| `maxSpeed` | number    | :material-checkbox-blank-circle-outline: | `1.6`                                   | maximum speed at which the player can loot (1.0 = normal speed)   |

??? success "Returns"
    | Data Type                            | Description
    | ------------------------------------ |-------------
    | id | The marker id
    | obj | The trolly object

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    local coords = GetEntityCoords(PlayerPedId())
    local tcoords = GetOffsetFromEntityInWorldCoords(PlayerPedId(), 0.0, 2.0, 0.0)

    CreateTrolly("cash", tcoords, function()
        print("Pickuped cash")
    end)
    ```