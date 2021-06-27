# DevMode
Only for development, turn on the log for anything done by the utility

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Status`                | boolean | :material-checkbox-blank-circle: | `-` | Turn on or off the devmode
| `Time`                | boolean | :material-checkbox-blank-circle-outline: | `true` | Turn on or off the time off the log
| `Format`                | string | :material-checkbox-blank-circle-outline: | `%s %s %s` | The [formatting](http://www.cplusplus.com/reference/cstdio/printf/) for the log

!!! success ""
    Dont need to be called every frame
---
??? example
    The **first** is the **action**, the **second** the **type**, the **third** the **id**
    ```
    DevMode(true, true, "%s | %s | %s")
    ```
    ![image](https://i.postimg.cc/6QW27jg2/image.png)<br>
                                                                                                   ^                         ^                       ^<br>
                                                                                              Action                 Type                   Id