---
name: Setting up Kuu-Kart
---
## Download SRB2Kart

Go to the [Official Release Thread](https://mb.srb2.org/threads/srb2kart.25868/) and download the full installer for windows. Alternatively, [Click this link](https://github.com/STJr/Kart-Public/releases/download/v1.3/srb2kart-v13-Installer.exe) to download the installer directly from GitHub.

## Install SRB2Kart

Run the installer and make sure to install it to a directory other than your Program Files folder.  
For example: `C:/Games/SRB2Kart` is a good location. `C:/Program Files (x86)/SRB2Kart` is not.

## Download Moe-Mansion

[Moe Mansion](https://mb.srb2.org/addons/srb2kart-1-3-moe-mansion.42/) is a custom build that works on top of the regular SRB2Kart application that enables some very quality of life changes, like frame interpolation and custom resolutions. [Click this link](https://kart.moe/moe-mansion/32-bit/srb2kart-moe.exe) to download Moe-Mansion, and place it directly into your SRB2Kart folder.

## Configure Startup

With Moe Mansion installed, we will want to make sure we launch SRB2Kart using the new executable, and in OpenGL mode. Inside the SRB2Kart folder, there should be two `.bat` files - `SRB2Kart (OpenGL).bat` and `SRB2Kart (Standard).bat`. You can delete the `Standard` one.

Open `SRB2Kart (OpenGL).bat` using any text editor, and replace the contents with the following  
*(change `width` and `height` values to your monitor's resolution)*:

```
@echo off
srb2kart-moe.exe -opengl -width 2560 -height 1440 -borderless
```

**From now on, always run SRB2Kart using this .bat file.**

## Configure Settings

From here, we can now configure the game's settings. Some important ones to consider are in the following locations:

* Options
  * Video Options
    * **Frame Interpolation**: On, Capped *// uncapped does nothing gameplay wise besides big number*
    * **Max Level Framerate**: 144 *// set this to your monitor's refresh rate*
    * **Future Sight**: Off/Full *// Interpolation adds ~30ms of display latency in order to smooth things out. Future Sight uses Extrapolation to guess and get that ~30ms of display latency back, but some things may not appear correctly near slopes.*
      * OpenGL Settings
        * **3D Models**: Off
        * **Fallback Player 3D Model**: Off
        * **Shaders**: On
        * **Texture Quality**: 32 Bits
        * **Texture Filter**: Nearest
        * **Anisotropic**: 16
        * **Wall Contrast Settings**: Standard
        * **Sprite Billboarding**: On
        * **Software Perspective**: Off
        * **Rendering Distance**: Max
  * Bird
    * Screen Tilting
      * Turn everything in here off. 


## Setup Addons

In your SRB2Kart folder, create a new folder called `DOWNLOAD`. From here, [Download and extract the contents of this zip file](https://drive.google.com/file/d/1_iplyy5VRRt3NugOZLU6bYffRLDPEx2o/view?usp=sharing) into the `DOWNLOAD` folder.

## Connect to the Dedicated Server

Scroll down to `Multiplayer`, then go to `Specify IPv4 Address`. From there, type in the following:

`kart.kuenaimaku.dev`

Hit enter. After a bit, you should connect to the server and have 116 addons checked. Once in, you can hit the menu key (`ESC` on kb+m, `START` on xbox controllers) and scroll down to `Player Setup...` to change your name, set your character, and pick a color.
