# C.R.A.F.TD
Creative Regeneration Assistance For TD(Technical Drawing)

Simple Minecraft-inspired CAD written in Python and Pyglet, inspired by Fogleman's version.

## Goals and Vision

I would like to see this project turn into an educational tool for TD. Kids love Minecraft and Python is a great first language.
This is a good opportunity to get children excited about programming and architecture.

The code should become well commented and more easily configurable. It should be easy to make some simple changes
and see the results quickly.

I think it would be great to turn the project into more of a library / API... a Python package that you import and then
use / configure to setup a world and run it. Something along these lines...


```python
import mc

world = mc.World(...)
world.set_block(x, y, z, mc.DIRT)
mc.run(world)
```

The API could contain functionality for the following:

- Easily configurable parameters like gravity, jump velocity, walking speed, etc.
- Hooks for terrain generation.

## How to Run

### Mac

On Mac OS X, you may have an issue with running Pyglet in 64-bit mode. Try running Python in 32-bit mode first:

```shell
arch -i386 python main.py
```

If that doesn't work, set Python to run in 32-bit mode by default:

```shell
defaults write com.apple.versioner.python Prefer-32-Bit -bool yes 
```

This assumes you are using the OS X default Python.  Works on Lion 10.7 with the default Python 2.7, and may work on other versions too.  Please raise an issue if not.
    
Or try Pyglet 1.2 alpha, which supports 64-bit mode:  

```shell
pip install https://pyglet.googlecode.com/files/pyglet-1.2alpha1.tar.gz 
```

### If you don't have pip or git

For pip:

- Mac or Linux: install with `sudo easy_install pip` (Mac or Linux) - or (Linux) find a package called something like 'python-pip' in your package manager.
- Windows: [install Distribute then Pip](http://stackoverflow.com/a/12476379/992887) using the linked .MSI installers.

For git:

- Mac: install [Homebrew](http://mxcl.github.com/homebrew/) first, then `brew install git`.
- Windows or Linux: see [Installing Git](http://git-scm.com/book/en/Getting-Started-Installing-Git) from the _Pro Git_ book.

See the [wiki](https://github.com/fogleman/Minecraft/wiki) for this project to install Python, and other tips.

## How to Play

### Moving

- W: forward
- S: back
- A: strafe left
- D: strafe right
- Mouse: look around
- Space: jump
- Tab: toggle flying mode

### Building

- Selecting type of block to create:
    - 1: brick
    - 2: grass
    - 3: sand
- Mouse left-click: remove block
- Mouse right-click: create block

### Quitting

- ESC: release mouse, then close window

I want to take no credit from Fogleman's craft, this project started out as a bet I made with a friend, that I could build the same app with different code in a night, turned out,
it was pretty easy. I cloned my repository and merged it with Fogleman's code and make a decent and fast version, and I just want it to be accessible in areas where it us most needed
, around school.



