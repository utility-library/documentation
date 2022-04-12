# SetVehicleWheelsPowered
Gives or takes power (energy) away from the wheels of the vehicle, simply if put on false the wheels of the vehicle will not turn anymore

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Vehicle`                | vehicle | :material-checkbox-blank-circle: | `-` | The vehicle
| `Active`                | boolean | :material-checkbox-blank-circle: | `-` | If its true give power to the wheels, otherwise remove the power from the wheels

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    SetVehicleWheelsPowered(veh, false)
    ```