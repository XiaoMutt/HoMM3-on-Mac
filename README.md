# HoMM3-on-Mac
How to play HoMM3 on Mac 64-bit OS
Using VirtualBox and Windows 7

This been tested on 27''inch iMac, and works very well.
Same setting may work on a Ubuntu virtual machine with Wine HD.

# Requirements
- Heroes of Might and Magic® 3: Complete (can be purchased on GOG.com)
- HoMM3 HD Patch
- Windows 7 32-bit
- VirtualBox

# Install and Setup Windows 7 VirtualBox Machine 
- Follow instructions of the VirtualBox installer
- Create a new virtual Windows7 machine with the following parameters
  - 3GB Memory
  - PS/2 Mouse
  - 8 CPUs **(Important!)**
  - HyperV interface and nested paging
  - 256 MB Video Memory
- Follow instructions to install Windows 7
- Install HoMM3 and it's patches
- Install HoMM3 HD path **(Important!)**
  - Without HoMM3 HD the game won't run, the orginal launcher will error out.
  - It also add many additional features to the game
- Make sure VirtualBox machine menu: Input->mouse Integration is checked

# Adjust Windows 7 and HoMM3 HD Launcher
- Change Windows 7 resolution to 1680x1050
  - This can be done using VirtualBox Machine Menu
  - Check View->Scaled Mode
  - Check View->Auto Resize Guest Display
  - Go View->Virtual Screen->choose the resolution
  - After this, uncheck Auto Resize Guest Display, and check Full Screen Mode
- Run HoMM3 HD and Configure
  - Mode: (strechable) 32-bit GDI
  - Source Size: 1064x798
  - Strech Filter: xBRZx2 + Bilinear + Sharpen
  - Render Threads: 8 **(Important!)**
  - Check System Cursor
  - Check Full Screen Mode
  - Check no CD/DVD
  - Check HD+
 
 # Run Game thourgh HoMM3 HD
 - In Mac OS Settings->Displays->(Hold Option Key) Click Scale->Choose 1280x720
 - Start Windows 7 virtual machine
 - Start HoMM3 HD and click "Play"
 - The game will not cover the whole screen and the black boarders ensure that the mouse will not trigger VirtualBox Menu or the Mac OS Launcher bar.
 - If mouse click stop working (this happens rarely),
  - VirtualBox menu->Input->uncheck Mouse Integration
  - Click somewhere in the game
  - Press VirtualBox Host Key, and re-check menu->Input->Mouse Integration
