SDL and minGW32



For windows download SDL from http://libsdl.org/ and add SDL2.dll and sdl2-config to C:\MinGW\bin and put the download in a folder like C:\Development.

To compile your program you must specify the include and lib folder for SDL2. In my example I used the following flags:

g++ main.cpp -IC:\Development\i686-w64-mingw32\include\SDL2 -LC:\Development\i686-w64-mingw32\lib -w -Wl,-subsystem,windows -lmingw32 -lSDL2main -lSDL2 -o SDLMain