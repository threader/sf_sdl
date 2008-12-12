this is port of SDL 1.2.13 to amigaos 68k from Bernd Rösch
This use the directory structure of SDL so a port to newer versions is easy.
The old amiga SDL 1.2.6 files are currently in the main tree, if maybe something must compare and fail under new versions. 

there are many fixes, timer and semaphore working correct, and faster speed.

A HotKey is add CTRL+ALT+H.If press only every 2. second frame is draw to GFX Card.

this give better playable results on slow amigas because a game that is written for 30 fps need now only transfer 15 fps to gfx card to work at correct speed.