###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_HINT_ROG_GAMEPAD_MICE_EXCLUDED

A variable containing a list of devices that are not ROG gamepad capable mice.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_ROG_GAMEPAD_MICE_EXCLUDED "SDL_ROG_GAMEPAD_MICE_EXCLUDED"
```

## Remarks

This will override [SDL_HINT_ROG_GAMEPAD_MICE](SDL_HINT_ROG_GAMEPAD_MICE)
and the built in device list.

The format of the string is a comma separated list of USB VID/PID pairs in
hexadecimal form, e.g.

`0xAAAA/0xBBBB,0xCCCC/0xDDDD`

The variable can also take the form of "@file", in which case the named
file will be loaded and interpreted as the value of the variable.

This hint should be set before SDL is initialized.

## Version

This hint is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

