SDL1.2.13 Version2 GCC linkerlibs

*  sdl Threads can now work with ixemul, this allow much more programs get working.
   sdl for working with libnix is named as libsdl_libnix.a and attached in adchive

*  Joystick that is default on SDL Port 0 use now Amiga Port 1 so you need not remove your mouse and plug joystick in. 
    the second joystick use then Port 0

*  SDL_HWSURFACE work now on rgb16 and rgb32 bgra32 screen mode and give 2-3* more speed in defendguin and work more systemfriendly
   on a bitmap that is later copy with AOS blitbitmaprastport on GFX Card to window.So windows on top of SDL windows are now correct visible
   resize of window work now with overlays.
*  audio with more than 2 channels can play and surround is now correct convert to 2 channels. 
   on 8 bit fullscreen mode YUV overlay play now fast 256 color grey video

* ahi use Unit 3 so you can define here a low quality setting for faster speed, withot touch your default setting

* SDL opengl work now with stormmesa and quarktex(winuae HW3d opengl) and if you have Warp3d HW also it use Warp3d HW.note the limit on Voodoo3 of textures to 256*256 is 
  here, but if the game have all images in png files you can convert images to be 256*256.they look of course not so sharp after convert, but game can play fast.
  Note: need link with libgl.a(attached).If you dont want opengl, you can use libgl_dummy.a(attached)
  You need also the new includes copy to your sdl dir. 

* check if enough memory is here before allocbitmap, so it handle low memory situitions better now.

----------------------------------------------------------
this is port of SDL 1.2.13 to amigaos 68k 
This use the directory structure of SDL so a port to newer versions is easy.
The old amiga SDL 1.2.6 files are currently in the main tree, if maybe something must compare and fail under new versions. 

there are many fixes, timer and semaphore working correct, and faster speed.

A HotKey is add CTRL+ALT+H.If press only every 2. second frame is draw to GFX Card.

this give better playable results on slow amigas because a game that is written for 30 fps need now only transfer 15 fps to gfx card to work at correct speed.

IMPORTANT: Use the new includes, this work too on old SDL 

sources can download here

http://amiga.svn.sourceforge.net/viewvc/amiga/