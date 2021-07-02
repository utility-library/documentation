# ReplaceTexture
Replace a texture of a model

| Argument              | Data Type                            | Nedeed                    | Default         | Description
| ----------------------| ------------------------------------ | ------------------------- |-----------------|-------------
| `Model`                | string | :material-checkbox-blank-circle: | `-` | The model to replace the texture
| `Texture Name`                | string | :material-checkbox-blank-circle: | `-` | The original texture name, you can found it with OpenIV
| `Url`                | string | :material-checkbox-blank-circle: | `-` | The url of the texture, can be a: .gif, .png, .jpg or a website (it can also be a nui)
| `Width`                | number | :material-checkbox-blank-circle: | `-` | The width of the texture
| `Height`                | number | :material-checkbox-blank-circle: | `-` | The height of the texture

!!! success ""
    Dont need to be called every frame
---
??? example
    ```
    ReplaceTexture("v_corp_facebeanbagd", "km_xj_v_beanbag", "https://gifer.com/en/embed/SBMP", 300, 300)
    ```
    <iframe src="https://streamable.com/e/efjtqw?autoplay=1&nocontrols=1" width="350" height="197" frameborder="0" allowfullscreen allow="autoplay"></iframe>
    <br>*If dont start [click me](https://streamable.com/e/efjtqw)*

??? info "How to find the texture name"
    Download [OpenIV and setup it](https://youtu.be/vwzSnbHfJeI) (follow the video until 3:50)

    ---

    When you are on OpenIV turn on the `Edit Mode` (in the top-right)
    ![https://i.postimg.cc/bJCzv82r/image.png](https://i.postimg.cc/bJCzv82r/image.png)
    
    Click `Yes`

    ---
    
    Ok, search the model name of the prop you want to find the texture name, for the tutorial i use this prop: v_corp_facebeanbagd<br>
    ![https://i.postimg.cc/26KDDwPB/image.png](https://i.postimg.cc/26KDDwPB/image.png)

    And click `Search "v_corp_facebeanbagd"`
    ![https://i.postimg.cc/rphmD5Bq/image.png](https://i.postimg.cc/rphmD5Bq/image.png)

    Wait that OpenIV search in the all directory the prop you have choose and then **double** click on the `v_corp_facebeanbagd.ydr` or `v_corp_facebeanbagd.yft`

    ---

    For me is a ydr<br>
    ![https://i.postimg.cc/yYzVYfDF/image.png](https://i.postimg.cc/yYzVYfDF/image.png)

    ---

    Ok, now open the file, a model will show up
    ![https://i.postimg.cc/2y0TJcJP/image.png](https://i.postimg.cc/2y0TJcJP/image.png)

    Click on `View embedded textures` in the bottom-right

    ---

    Some texture will show up, you need to choose the right texture, for me there is only one
    ![https://i.postimg.cc/vDRDQMp9/image.png](https://i.postimg.cc/vDRDQMp9/image.png)

    So, we have finished, `km_xj_v_beanbag` is the textureName