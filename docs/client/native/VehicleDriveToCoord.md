# TaskVehicleDriveToCoord
ask to a ped with a vehicle to drive at a specific coordinate

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Ped`                | ped | :material-checkbox-blank-circle: | `-` | The driver of the vehicle
| `Vehicle`                | vehicle | :material-checkbox-blank-circle: | `-` | The vehicle
| `Destination`                | vector3 | :material-checkbox-blank-circle: | `-` | The destination coords
| `Speed`                | number | :material-checkbox-blank-circle-outline: | `10.0` | The driving speed
| `Stop range`                | number | :material-checkbox-blank-circle-outline: | `1.0` | The stop range

!!! success ""
    Dont need to be called every frame
---
??? example
    Using **vector3**
    ```
    TaskVehicleDriveToCoord(ped, vehicle, vector3(0.0, 0.0, 0.0))
    ```
??? abstract "Old method"
    ```
    TaskVehicleDriveToCoord(ped, vehicle, vector3(0.0, 0.0, 0.0), 10.0, 0, GetEntityModel(vehicle), driving_style, 1.0)
    ```
    ???+ bug "Old problem"
        **THE DRIVING STYLE!!**<br>is something almost impossible to find, there is almost 0 documentation about the driving style, every time i tried to use this native i always had to go and grab the driving style from other scripts

    ??? info "Using old native"
        although i dont recommend it, you can use the old native via `old_TaskVehicleDriveToCoord`