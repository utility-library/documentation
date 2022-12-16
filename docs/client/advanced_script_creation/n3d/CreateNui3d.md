# CreateNui3d
Create a 3d nui in the game, simply render a html page in a DUI

| Argument    | Data Type | Needed                                   | Default | Description                    |
|-------------|-----------|------------------------------------------|---------|--------------------------------|
| `GFXName`   | string    | :material-checkbox-blank-circle:         | `-`     | The name of your .gfx render   |
| `Directory` | anything  | :material-checkbox-blank-circle-outline: | `-`     | The directory of the html file |

!!! success ""
    Dont need to be called every frame

???+ success "Returns"
    | Child     | Data Type | Description              |
    |-----------|-----------|---------------------------------------|
    | [N3dClass](../N3dClass)      | class    | The nui 3d class to interact with the n3d (click on [N3dClass](#N3dClass) to see the class method)
    | handle      | number    | The handle for interact with the n3d |
---
??? example
    ??? info "With class"
        ```
        local n3d = CreateNui3d("utility_lib_1", "html/ui.html")

        n3d:show(vector3(0.0, 0.0, 0.0))
        ```
    ??? info "With function"
        ```
        local _, n3dHandle = CreateNui3d("utility_lib_1", "html/ui.html")

        Show3dNui(n3dHandle, vector3(0.0, 0.0, 0.0))
        ```
    ??? info "My first project with the n3d"
        I created a ammo hud with the n3d and its amazing, is like an object, but also like an nui,<br>sincerely i love this thing!
    
        <iframe src="https://streamable.com/e/rzrbw9?nocontrols=1" width="682" height="383" frameborder="0" allowfullscreen allow="autoplay"></iframe>
        <br>*If dont start [click me](https://streamable.com/e/rzrbw9)*<br><br>
        You can found this script here > https://forum.cfx.re/t/release-utility-ammohud/4291362