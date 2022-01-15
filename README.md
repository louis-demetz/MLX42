# MLX42

Project still WIP!

My own recreation of the MiniLibX library used by 42, using glfw &amp; glad, running on OpenGL 3.3.
The goal of MLX42 is to replace the outdated and stale MiniLibX library.

## Differences to MiniLibX
#### No Images
Instead of having separate "Images" (textures) theres only a single buffer used to draw the pixels.

#### Custom XPM (XPM42) format
A custom simple to use XPM-like format which is has some minor differences to the XPM3 format.

#### Cross-Platform
The main idea of MLX42 is to be a cross-platform graphics interface, in 42 everything runs (currently) on MacOS but its
very useful to be able to work remotley on different machines. With MiniLibX this is not possible.

#### Misc
 - Yes, MLX42 adheres 99.98% to the latest norme. 
 - 100% Documented, making it very beginner friendly and easy to use.
 - Running with OpenGL 3.3
 
## Installation

### For MacOS:
1. Download MLX42 & Build
```bash 
➜  ~ git clone https://github.com/W2Codam/MLX42.git
➜  ~ make
```
2. Create a ```main.c``` file, include ```MLX42/MLX42.h```, compile with ```-lglfw```.
3. Run.

The systems below have not been tested yet.

### For Linux:

1. Download GLFW: [Click Me!](https://github.com/glfw/glfw/releases/download/3.3.6/glfw-3.3.6.zip)
2. Extract GLFW, and to install, run the following commands:
```bash 
➜  ~ sudo apt update
➜  ~ sudo apt install build-essential
➜  ~ sudo apt install cmake

# NOTE: Navigate to the directory where you extracted GLFW!

➜  ~ sudo apt install xorg-dev
➜  ~ cmake -G "Unix Makefiles"
➜  ~ make
➜  ~ sudo make install
➜  ~ sudo apt-get install libx11-dev libglu1-mesa-dev freeglut3-dev libglew1.5 libglew1.5-dev libglu1-mesa libgl1-mesa-glx libgl1-mesa-dev libglfw3-dev libglfw3
```

3. Download MLX42 & Build
```bash 
➜  ~ git clone https://github.com/W2Codam/MLX42.git
➜  ~ make
```
4. Create a ```main.c``` file, include ```MLX42/MLX42.h```, compile with:
 - ```-ldl -lglfw -lGL -lX11 -lpthread -lXrandr -lXi```
5. Run.

### For Windows:
- Switch to MacOS or Linux, as there is no CMake or way to compile for it yet.
