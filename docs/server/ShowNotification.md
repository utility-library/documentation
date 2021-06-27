# ShowNotification
Draw a notification in the bottom-left

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Source`                | number | :material-checkbox-blank-circle: | `-` | The id to which the notification must be sent
| `Message`                | string | :material-checkbox-blank-circle: | `-` | The message to show

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    ShowNotification(source, "Example")
    ```
??? tip
    ## Supported Color Syntax

    | Syntax | Color           |
    |--------|-----------------|
    | ~r~    | <p style="color:red">Red</p>             |
    | ~b~    | <p style="color:deepskyblue">Blue</p>            |
    | ~g~    | <p style="color:springgreen">Green</p>           |    
    | ~y~    | <p style="color:yellow">Yellow</p>          |
    | ~p~    | <p style="color:darkviolet">Purple</p>          |
    | ~o~    | <p style="color:darkorange">Orange</p>          |
    | ~c~    | <p style="color:darkgrey">Grey</p>            |
    | ~m~    | <p style="color:grey">Dark Grey</p>       |
    | ~u~    | <p style="color:black">Black</p>           |
    | ~n~    | New Line        |
    | ~s~    | White (default) |
    | ~w~    | White           |
    | ~h~    | **Bold**     |
    | ∑      | Rockstar Icon |
    | ¦      | Rockstar Verified Icon |
    `ShowNotification("∑÷¦~r~ r ~b~ b ~g~ g ~y~ y ~p~ p ~c~ gr ~m~ d gr ~u~ bl ~o~ or ~s~ re ~n~ nl ~h~ Bold")` | ![image](https://i.postimg.cc/3NWNbsCs/7Ev44Yc.png)


