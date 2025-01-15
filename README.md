# ICS415_Project1
Ray Tracer Program

This is a ray tracer program for drawing on a canvas. The program is currently in its early stages. The scene is made up of 3 differently colored spheres. The program draws on the canvas what it can see in scene. The camera is in the center of the scene (0, 0, 0). There are 3 spheres, and they are located in (0, -1, 3), (2, 0, 4) and (-2, 0, 4).

How it works:
	The program generates a ray for each pixel, and its direction is based on the pixel coordinates. The rays are casted from the camera through the view port (1x1). The sphere is a set of points that share a center that has equal distance between all points. The rays are used to generate a linear equation. The color of the pixel is determined by the solution of the system of equations composed of the linear equation and the sphere equations. The closet solution is selected. If there is no solution, then the ray has not passed throgh any sphere (white background).

Compiling and running:
	The compiler used to test and run the program is Clang with C++11.
	Simply compile main.cc (no external libraries required), then run the executable. The program will generate a 256x256 bitmap image file of the scene. The file is named image.bmp.

Changelog:
	15/1/2025: First Assignment Done.