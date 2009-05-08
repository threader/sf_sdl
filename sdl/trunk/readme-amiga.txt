SDL1.2.13 Version2 linkerlib

SDL_HWSURFACE work now on rgb16 and rgb32 bgra32 screen mode and give 2-3* more speed in defendguin and work more systemfriendly
on a bitmap that is later copy with AOS blitbitmaprastport on GFX Card to window.So windows on top of SDL windows are now correct visible
resize of window work now.
audio with more than 2 channels can play and surround is now correct convert to 2 channels.(merge 6 lines in from powersdl)  

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