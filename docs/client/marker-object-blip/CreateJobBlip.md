# CreateJobBlip
Create a blip for a specific job. (auto-update)

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Name`                | string/number | :material-checkbox-blank-circle: | `-` | The name of the blip
| `Coords`                | vector3 | :material-checkbox-blank-circle: | `-` | The coordinates to create the blip
| `Job`                | string | :material-checkbox-blank-circle: | `-` | The job that can see the blip
| `Sprite`                | number | :material-checkbox-blank-circle: | `-` | The [sprite ID](https://wiki.gtanet.work/index.php?title=Blips)
| `Colour`                | number | :material-checkbox-blank-circle: | `-` | The [colour ID](https://wiki.gtanet.work/index.php?title=Blips#Blip_Colors)
| `Scale`                | number | :material-checkbox-blank-circle-outline: | `1.0` | The scale of the blip
    
!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    CreateJobBlip("My Blip", vector3(0.0, 0.0, 0.0), "police", 11, 2)
    ```