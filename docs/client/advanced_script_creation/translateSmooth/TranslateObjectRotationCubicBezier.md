# TranslateObjectRotationCubicBezier
Rotate an entity based on a [cubic bezier](https://en.wikipedia.org/wiki/Bézier_curve).
Is a little "advanced" logic to explain how it works in a nutshell.
You can also use https://cubic-bezier.com (select the arrow next to copy and copy the last one, remember to add a 0 before the numbers)

??? info
    Thanks to https://github.com/gre/bezier-easing for the incredible math behind this, i just converted the code to lua and did the NEWTON_MIN_SLOPE tweening, since precision rounding in lua seems to be different than in js.

| Argument        | Data Type    | Needed                           | Default | Description                                                                                                                      |
|-----------------|--------------|----------------------------------|---------|----------------------------------------------------------------------------------------------------------------------------------|
| `obj`           | object       | :material-checkbox-blank-circle: | `-`     |                                                                                                                                  |
| `destination`   | vector3      | :material-checkbox-blank-circle: | `-`     | The destination coords, you can also use [GetOffsetFromEntityInWorldCoords](https://docs.fivem.net/natives/?_0x1899F328B0E12848) |
| `duration`      | number       | :material-checkbox-blank-circle: | `-`     | Total duration in ms                                                                                                             |
| `rotationOrder` | number       | :material-checkbox-blank-circle: | `-`     | The order yaw, pitch and roll is applied. Usually 2. Read more [here](https://docs.fivem.net/natives/?_0xAFBD61CC738D9EB9)       |
| `cubicBezier`   | table/string | :material-checkbox-blank-circle: | `-`     | A table containing the 2 points or one of the predefined cubic beziers                                                           |

!!! success ""
    Dont need to be called every frame

???+ example "Predefined cubic beziers"
    | Name | Description |
    | ---- | --- |
    | ease | Indicates that the interpolation starts slowly, accelerates sharply, and then slows gradually towards the end. This keyword represents the easing function cubic-bezier(0.25, 0.1, 0.25, 1.0). It is similar to ease-in-out, though it accelerates more sharply at the beginning. |
    | easeIn | Indicates that the interpolation starts slowly, then progressively speeds up until the end, at which point it stops abruptly. This keyword represents the easing function cubic-bezier(0.42, 0.0, 1.0, 1.0). |
    | easeOut | Indicates that the interpolation starts abruptly and then progressively slows down towards the end. This keyword represents the easing function cubic-bezier(0.0, 0.0, 0.58, 1.0). |
    | easeInOut | Indicates that the interpolation starts slowly, speeds up, and then slows down towards the end. This keyword represents the easing function cubic-bezier(0.42, 0.0, 0.58, 1.0). At the beginning, it behaves like the ease-in keyword; at the end, it is like the ease-out keyword. |

    [Source of descriptions](https://developer.mozilla.org/en-US/docs/Web/CSS/easing-function)
---
??? example
    ??? info "With Predefined Cubic Bezier"
        ```
        local rot = GetEntityRotation(obj, 2)

        TranslateObjectRotationCubicBezier(obj, rot + vec3(0.0, 0.0, 90.0), 5000, 2, "ease")
        ```
    ??? info "With Custom Cubic Bezier"
        ```
        local rot = GetEntityRotation(obj, 2)

        TranslateObjectRotationCubicBezier(obj, rot + vec3(0.0, 0.0, 90.0), 5000, 2, {0.0, 0.9, 1.0, 1.0})
        ```