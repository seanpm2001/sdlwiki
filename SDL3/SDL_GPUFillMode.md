###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GPUFillMode

Specifies the fill mode of the graphics pipeline.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
typedef enum SDL_GPUFillMode
{
    SDL_GPU_FILLMODE_FILL,  /**< Polygons will be rendered via rasterization. */
    SDL_GPU_FILLMODE_LINE   /**< Polygon edges will be drawn as line segments. */
} SDL_GPUFillMode;
```

## Version

This enum is available since SDL 3.1.3

## See Also

- [SDL_CreateGPUGraphicsPipeline](SDL_CreateGPUGraphicsPipeline)

----
[CategoryAPI](CategoryAPI), [CategoryAPIEnum](CategoryAPIEnum), [CategoryGPU](CategoryGPU)

