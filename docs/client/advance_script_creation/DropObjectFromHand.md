# DropObjectFromHand (Client side)
Drop the object that was taken via the [TakeObjectOnHand](127.0.0.1:8000/md/client/5_advance_script_creation/TakeObjectOnHand.md)

| Argument              | Data Type                            | Nedeed                    | Default                       | Description
| ----------------------| ------------------------------------ | ------------------------- |-------------------------------|-------------
| `Entity`                | entity | :material-checkbox-blank-circle: | `-` | The entity
| `Delete`                | boolean | :material-checkbox-blank-circle-outline: | `false` | Delete or no the entity when dropped

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    DropObjectFromHand(entity, false)
    ```    
    <img src="https://i.postimg.cc/fTk8H7T0/image.png" alt="" width="40%" heigth="40%"/>
