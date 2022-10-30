# Decker on Linux
 Instructions for building and installing Decker on Linux

 [Decker](https://beyondloom.com/decker/index.html) is an interactive media platform in the spirit of HyperCard. It comes in two versions, one that runsin a web browser as a [web page](http://beyondloom.com/decker/tour.html) and one that runs independantly. This is a guide on how to install the independant version on Linux.

 ## Fork
Decker is hosted on GitHub, so first step is to [download the code](https://github.com/JohnEarnest/Decker) from there.

## Prepare
 Open a terminal emulator and install SDL2 and SDL_image. On Ubuntu and Debian that can be done uning APT:
`sudo apt install libsdl2-2.0-0 libsdl2-dev libsdl2-image-dev`

## Build
Navigate to the Decker folder and run the following command to compile decker:
  * `make decker`
 
## Install
Install Decker on your computer by running the following command:
*  `sudo make install`

(This copies decker to `/usr/local/bin/`)

 ## GUI launcher
Decker is now installed and can be run by writing `decker` in the terminal emulator. To lauch it graphically we need two more files from this ([decker-linux](https://github.com/1jss/decker-linux)) repo.

* Copy `decker.png` to the folder `/usr/share/icons/hicolor/64x64/apps/`
* Copy `decker.desktop` to the folder `/usr/share/applications/`

Now Decker should show up in your GUI launcher! Have fun!
