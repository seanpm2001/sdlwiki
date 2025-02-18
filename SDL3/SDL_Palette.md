###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_Palette

A set of indexed colors representing a palette.

## Header File

Defined in [<SDL3/SDL_pixels.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_pixels.h)

## Syntax

```c
typedef struct SDL_Palette
{
    int ncolors;        /**< number of elements in `colors`. */
    SDL_Color *colors;  /**< an array of colors, `ncolors` long. */
    Uint32 version;     /**< internal use only, do not touch. */
    int refcount;       /**< internal use only, do not touch. */
} SDL_Palette;
```

## Version

This struct is available since SDL 3.1.3.

## See Also

- [SDL_SetPaletteColors](SDL_SetPaletteColors)

----
[CategoryAPI](CategoryAPI), [CategoryAPIStruct](CategoryAPIStruct), [CategoryPixels](CategoryPixels)

