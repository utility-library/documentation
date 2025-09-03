# ButtonNotification
Shows a notification in the top-right that support the displaying button inputs

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Message`                | string | :material-checkbox-blank-circle: | `-` | The message to show
| `Beep`                | boolean | :material-checkbox-blank-circle-outline: | `true` | The beep sound on msg update


!!! danger ""
    Need to be called every frame
---
??? example
    ```
    ButtonNotification("Example")
    ```
??? tip
    If you write `{any_letter}` the content will be converted to button inputs<br>

    ---
    
    **Example**:<br>`ButtonNotification("A simple message {X} {D}")`<br>
    
    **Result**:<br>![https://i.postimg.cc/XJ7dWFk3/DcxWl3r.png](https://i.postimg.cc/XJ7dWFk3/DcxWl3r.png)

