###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetJoystickPathForID

Get the implementation dependent path of a joystick.

## Header File

Defined in [<SDL3/SDL_joystick.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_joystick.h)

## Syntax

```c
const char * SDL_GetJoystickPathForID(SDL_JoystickID instance_id);
```

## Function Parameters

|                                  |                 |                           |
| -------------------------------- | --------------- | ------------------------- |
| [SDL_JoystickID](SDL_JoystickID) | **instance_id** | the joystick instance ID. |

## Return Value

(const char *) Returns the path of the selected joystick. If no path can be
found, this function returns NULL; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

This can be called before any joysticks are opened.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_GetJoystickPath](SDL_GetJoystickPath)
- [SDL_GetJoysticks](SDL_GetJoysticks)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

