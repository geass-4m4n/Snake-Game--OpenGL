# SnakeGL
Popular snake game in C
![alt tag](https://github.com/geass-4m4n/Snake-Game--OpenGL/blob/master/Screenshots/1s.png)

## COMPILE INSTUCTIONS
 
### Add GLFW and GL library to your /usr/include folder

1. Download GLFW source files from http://www.glfw.org/download.html
2. Install Build Dependencies by running 
```sh
$ sudo apt-get install cmake xorg-dev libglu1-mesa-dev
```
3. cd in GLFW directory downloaded in step 1
4. Run the command  in terminal 
```sh
$ cmake -G "Unix Makefiles"
$ sudo make
$ sudo make install
```
### Next step is to add glad libraries
1. Copy the glad and KHR folder into /usr/include/
2. Make sure to keep glad.c in the same directory as snake.cpp

### Compiling the program
1. cd into the cloned directory and run 
```sh
$ g++ -o snakegl snakegl.cpp glad.c -lglfw3 -lGL -lm -lXrandr -lXi -lX11 -lXxf86vm -lpthread -ldl -lXinerama -lXcursor
```
2. Run the project by 
```sh
$ ./snakegl
```

