# TranslateZAnimated
Animates the movement of an entity in the Z

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Object`                | object | :material-checkbox-blank-circle: | `-` | The object to which we need to apply the animation
| `Z`                | number | :material-checkbox-blank-circle: | `-` | How much to move the Z (if negative the object will go down)
| `Steps Duration`                | number | :material-checkbox-blank-circle-outline: | `10` | How much every step durate

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    TranslateZAnimated(ojb, -5)
    ```