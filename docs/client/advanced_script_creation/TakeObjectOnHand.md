<<<<<<< HEAD
# TakeObjectOnHand (Client side)
Take the object defined as an argument

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Ped`                | ped | :material-checkbox-blank-circle: | `-` | The ped that take the object
| `Entity`                | entity/string/hash | :material-checkbox-blank-circle: | `-` | The entity to take, you can pass the object handle or the model name/hash
| `zOffset`                | number | :material-checkbox-blank-circle-outline: | `0.2` | The z offset
| `xPos`                | number | :material-checkbox-blank-circle-outline: | `0.2` | The x position for the attachment
| `yPos`                | number | :material-checkbox-blank-circle-outline: | `0.08` | The y position for the attachment
| `zPos`                | number | :material-checkbox-blank-circle-outline: | `0.2` | The z position for the attachment
| `xRot`                | number | :material-checkbox-blank-circle-outline: | `-45.0` | The x rotation for the attachment
| `yRot`                | number | :material-checkbox-blank-circle-outline: | `290.0` | The y rotation for the attachment
| `zRot`                | number | :material-checkbox-blank-circle-outline: | `0.0` | The z rotation for the attachment


!!! success ""
    Dont need to be called every frame
---
??? example
    With the model name
    ```
    TakeObjectOnHand(PlayerPedId(), "prop_roadcone02a")
    ```
    With the entity handle
    ```
    TakeObjectOnHand(PlayerPedId(), obj)
    ```

    <img src="https://i.postimg.cc/hv4KFy3n/image.png" alt="" width="40%" heigth="40%"/>
=======
# TakeObjectOnHand (Client side)
Take the object defined as an argument

| Argument              | Data Type                            | Needed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Ped`                | ped | :material-checkbox-blank-circle: | `-` | The ped that take the object
| `Entity`                | entity/string/hash | :material-checkbox-blank-circle: | `-` | The entity to take, you can pass the object handle or the model name/hash
| `zOffset`                | number | :material-checkbox-blank-circle-outline: | `0.2` | The z offset
| `xPos`                | number | :material-checkbox-blank-circle-outline: | `0.2` | The x position for the attachment
| `yPos`                | number | :material-checkbox-blank-circle-outline: | `0.08` | The y position for the attachment
| `zPos`                | number | :material-checkbox-blank-circle-outline: | `0.2` | The z position for the attachment
| `xRot`                | number | :material-checkbox-blank-circle-outline: | `-45.0` | The x rotation for the attachment
| `yRot`                | number | :material-checkbox-blank-circle-outline: | `290.0` | The y rotation for the attachment
| `zRot`                | number | :material-checkbox-blank-circle-outline: | `0.0` | The z rotation for the attachment


!!! success ""
    Dont need to be called every frame
---
??? example
    With the model name
    ```
    TakeObjectOnHand(PlayerPedId(), "prop_roadcone02a")
    ```
    With the entity handle
    ```
    TakeObjectOnHand(PlayerPedId(), obj)
    ```

    <img src="https://i.postimg.cc/hv4KFy3n/image.png" alt="" width="40%" heigth="40%"/>
>>>>>>> 2a78759c92d8c3cfcceba1661317ce3c33c6f503
