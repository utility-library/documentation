# ButtonFor
Shows a notification in the top-right that support the displaying button inputs for a defined ms

| Argument              | Data Type                            | Needed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Message`                | string | :material-checkbox-blank-circle: | `-` | The message to show
| `Duration`                | number | :material-checkbox-blank-circle: | `-` | The duration time in milliseconds (**ms**)

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    ButtonFor("Example", 5000)
    ```
??? tip
    If you write `{any_letter}` the content will be converted to button inputs<br>

    ---
    
    **Example**:<br>`ButtonFor("A simple message {X} {D}", 5000)`<br>
    
    **Result**:<br>![https://i.postimg.cc/XJ7dWFk3/DcxWl3r.png](https://i.postimg.cc/XJ7dWFk3/DcxWl3r.png)
