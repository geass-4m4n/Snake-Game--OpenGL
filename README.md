# SnakeGL
Popular snake game in C
![alt tag](https://github.com/anubhawbhalotia/SnakeGL/blob/master/Screenshots/Screenshot%20Version%201.0.png)

## COMPILE INSTUCTIONS
 
### Add GLFW and GL library to your /usr/include folder
1. Download GLFW source files from http://www.glfw.org/download.html
2. Install Build Dependencies by running sudo apt-get install cmake xorg-dev libglu1-mesa-dev
3. cd in GLFW directory downloaded in step 2
4. Run the command cmake -G "Unix Makefiles" in terminal and then run sudo make and then sudo make install

### Next step is to add glad libraries
1. Copy the glad and KHR folder into /usr/include/
2. Make sure to keep glad.c in the same directory as pacmanGL.cpp

### Compiling the program
1. cd into the cloned directory and run g++ -o snakegl snakegl.cpp glad.c -lglfw3 -lGL -lm -lXrandr -lXi -lX11 -lXxf86vm -lpthread -ldl -lXinerama -lXcursor
2. Run the project by ./snakegl

