# StartParticleFxOnNetworkEntity
Create particles on a networked entity, obviously the particles will also be synchronized

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `ptxAsset`                | string | :material-checkbox-blank-circle: | `-` | The ptfx dictionary (core, etc..)
| `name`                | string | :material-checkbox-blank-circle: | `-` | The particle name
| `obj`                | number | :material-checkbox-blank-circle: | `-` | The client entity (not netid)
| `offset`                | vector3 | :material-checkbox-blank-circle: | `-` | 
| `rot`                | vector3 | :material-checkbox-blank-circle: | `-` | 
| `scale`                | number | :material-checkbox-blank-circle: | `-` | 
| `axis`                | number | :material-checkbox-blank-circle-outline: | `-` | 


!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    StartParticleFxOnNetworkEntity("scr_ornate_heist", "scr_heist_ornate_thermal_burn", thermal, vector3(0.0, 1.0, -0.1), vector3(0.0, 0.0, 0.0), 1.0)
    ```