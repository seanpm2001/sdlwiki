# CategoryCamera

Video capture for the SDL library.

This API lets apps read input from video sources, like webcams. Camera
devices can be enumerated, queried, and opened. Once opened, it will
provide [SDL_Surface](SDL_Surface) objects as new frames of video come in.
These surfaces can be uploaded to an [SDL_Texture](SDL_Texture) or
processed as pixels in memory.

## Camera gotchas

Consumer-level camera hardware tends to take a little while to warm up,
once the device has been opened. Generally most camera apps have some sort
of UI to take a picture (a button to snap a pic while a preview is showing,
some sort of multi-second countdown for the user to pose, like a photo
booth), which puts control in the users' hands, or they are intended to
stay on for long times (Pokemon Go, etc).

It's not uncommon that a newly-opened camera will provide a couple of
completely black frames, maybe followed by some under-exposed images. If
taking single frame automatically, or recording video from a camera's input
without the user initiating it from a preview, it could be wise to drop the
first several frames (if not the first several _seconds_ worth of frames!)
before using images from a camera.

<!-- END CATEGORY DOCUMENTATION -->

## Functions

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryCamera, CategoryAPIFunction -->
- [SDL_AcquireCameraFrame](SDL_AcquireCameraFrame)
- [SDL_CloseCamera](SDL_CloseCamera)
- [SDL_GetCameraDriver](SDL_GetCameraDriver)
- [SDL_GetCameraFormat](SDL_GetCameraFormat)
- [SDL_GetCameraID](SDL_GetCameraID)
- [SDL_GetCameraName](SDL_GetCameraName)
- [SDL_GetCameraPermissionState](SDL_GetCameraPermissionState)
- [SDL_GetCameraPosition](SDL_GetCameraPosition)
- [SDL_GetCameraProperties](SDL_GetCameraProperties)
- [SDL_GetCameras](SDL_GetCameras)
- [SDL_GetCameraSupportedFormats](SDL_GetCameraSupportedFormats)
- [SDL_GetCurrentCameraDriver](SDL_GetCurrentCameraDriver)
- [SDL_GetNumCameraDrivers](SDL_GetNumCameraDrivers)
- [SDL_OpenCamera](SDL_OpenCamera)
- [SDL_ReleaseCameraFrame](SDL_ReleaseCameraFrame)
<!-- END CATEGORY LIST -->

## Datatypes

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryCamera, CategoryAPIDatatype -->
- [SDL_Camera](SDL_Camera)
- [SDL_CameraID](SDL_CameraID)
<!-- END CATEGORY LIST -->

## Structs

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryCamera, CategoryAPIStruct -->
- [SDL_CameraSpec](SDL_CameraSpec)
<!-- END CATEGORY LIST -->

## Enums

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryCamera, CategoryAPIEnum -->
- [SDL_CameraPosition](SDL_CameraPosition)
<!-- END CATEGORY LIST -->

## Macros

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryCamera, CategoryAPIMacro -->
- (none.)
<!-- END CATEGORY LIST -->


----
[CategoryAPICategory](CategoryAPICategory)


