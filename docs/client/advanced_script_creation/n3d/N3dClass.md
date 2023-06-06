# N3d Class Methods
This is all of the methods for the n3d class

| Class            | Description                                                                                     |
|------------------|-------------------------------------------------------------------------------------------------|
| `init`           | Load the .gfx render to render a nui, width and height can be setted                            |
| `datas`          | Return a table with all the datas of the N3d (options and default datas)                        |
| `destroy`        | Delete the .gfx render and unload the scaleform, you need to do that if you don't need that n3d |
| `started`        | Return true if the .gfx render has finished to load anymore                                     |
| `show`           | Shows the n3d                                                                                   |
| `hide`           | Hides the n3d, but keeps the render active for later use                                        |
| `visible`        | Return true if the .gfx render and the n3d is visible                                           |
| `scale`          | You can change the scale of the whole rendering, it takes some knowledge in DUI                 |
| `rotation`       | The heading of the render                                                                       |
| `attach`         | Attach the n3d to the entity, accept some offsets                                               |
| `detach`         | Detach the n3d from the entity                                                                  |
| `object`         | Return the dui render                                                                           |
| `replaceTexture` | Replace a texture with this n3d (dui)                                                           |
| `msg`            | Send message to the dui render, can be use like the SendNuiMessage for update data on the n3d   |

???+ example "All classes arguments"
    ## Read the argument!

    ??? quote "init"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `directory`              | string  | `-` | The directory of the html file
        | `width`                  | number  | `1920` | The width of the render
        | `height`                  | number | `1080` | The height of the render

        ---

        ## Example
        ```
        n3d:init("html/ui.html")
        ```
    ??? quote "datas"
        !!! success "Returns"
            | Data Type                            | Description
            | ------------------------------------ |-------------
            | table | All the datas of the N3d (options and default datas)

        ---
        
        ## Example
        ```
        n3d:datas()
        ```
    ??? quote "destroy"
        ## Example
        ```
        n3d:destroy()
        ```
    ??? quote "started"
        !!! success "Returns"
            | Data Type                            | Description
            | ------------------------------------ |-------------
            | boolean | If is started or no

        ---

        ## Example
        ```
        n3d:started()
        ```
    ??? quote "show"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `coords`              | vector3  | `-` | The coords where the n3d need to be show
        | `scale`               | number  | `0.1` | The scale of the n3d (0.1 - 1.0)

        ---

        ## Example
        ```
        n3d:show(vector3(0.0, 0.0, 0.0))
        ```
    ??? quote "hide"
        ## Example
        ```
        n3d:hide()
        ```
    ??? quote "visible"
        !!! success "Returns"
            | Data Type                            | Description
            | ------------------------------------ |-------------
            | boolean | If is visible or no

        ---
        
        ## Example
        ```
        n3d:visible()
        ```
    ??? quote "scale"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `scale`              | vector3  | `-` | The new advanced scale of the DUI

        ---
        
        ## Example
        ```
        n3d:scale(vector3(1.0, 5.0, 3.0))
        ```
    ??? quote "rotation"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `rotation`              | number  | `-` | The rotation (0.0 - 360.0)
        | `withplayer`      | boolean  | `false` | If true add the custom rotation to the rotation of the player for sync the player heading, otherwise dont rotate with the player

        ---
        
        ## Example
        ```
        n3d:rotation(90.0)
        ```
    ??? quote "attach"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `entity`              | entity  | `-` | The entity to attach
        | `offset`      | vector3  | `vector3(0.0,0.0,0.0)` | The offset of the attachment (x, y, z)

        ---
        
        ## Example
        ```
        n3d:attach(entity)
        ```
    ??? quote "detach"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `At Coords`              | boolean  | `-` | If true, detach the n3d at the detachment coordinates, otherwise return to the last recorded coordinates

        ---
        
        ## Example
        ```
        n3d:detach()
        ```
    ??? quote "object"
        !!! success "Returns"
            | Data Type                            | Description
            | ------------------------------------ |-------------
            | Dui Handle | The rendering dui

        ---
        
        ## Example
        ```
        n3d:object()
        ```
    ??? quote "replaceTexture"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `dict`              | string  | `-` | The [texture dictionary](../../misc/ReplaceTexture.md)
        | `textureName`      | string  | `-` | The [texture name](../../misc/ReplaceTexture.md)

        ---
        
        ## Example
        ```
        n3d:replaceTexture("p_cs_cam_phone", "phone_screen")
        ```
    ??? quote "msg"
        | Argument              | Data Type                            | Default          | Description
        | ----------------------| ------------------------------------ | -----------------|-------------
        | `Msg`              | table  | `-` | The table to send at the n3d

        ---
        
        ## Example
        ```
        n3d:msg({
            show = true
        })
        ```

        ??? info "Listen the message"
            The listening of the messages sent by the msg method can be handled through javascript in html, like the nui.<br> Here below you can find an example

            ```
            window.addEventListener('message', function(event){		
                console.log(`Show is ` + event.data.show)
            })
            ```