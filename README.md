# teeworlds-xpanic
TeeWorlds mod "XPanic", remade by kurosio

Building on Linux or macOS (bam)
==========================

Installing dependencies
-----------------------

    # Debian/Ubuntu 19.10+
    sudo apt install bam git libfreetype6-dev libsdl2-dev libpnglite-dev libwavpack-dev python3
    
    # Fedora
    sudo dnf install bam gcc-c++ git freetype-devel pnglite-devel python3 SDL2-devel wavpack-devel
    
    # Arch Linux (doesn't have pnglite in its repositories)
    sudo pacman -S --needed base-devel bam freetype2 git python sdl2 wavpack
    
    # macOS
    brew install bam freetype sdl2
    
    # other (add bam to your path)
    git clone https://github.com/teeworlds/bam
    cd bam
    ./make_unix.sh


Downloading repository
----------------------

    git clone https://github.com/orchidalloy/teeworlds-xpanic.git
    cd teeworlds-xpanic
    
    # If you already cloned the repository before, use:
    # git submodule update --init


Building
--------

    cd teeworlds-xpanic
        Changes to the teeworlds-xpanic source directory
    ./bam/bam server_release
        Compiles xPanic (Server)
       
       
       
Available targets for release and debug (not tested):
--------

    release (for all in release mode)
    debug (for all in debug mode)
    server_release
    server_debug
    client_release
    client_debug
 
 The compiled game is located in teeworlds-xpanic
