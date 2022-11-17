# 3DViewer

Implementation of 3DViewer, program to view 3D wireframe models in the C++ programming language in the object-oriented programming paradigm. The models themselves loaded from .obj files and be viewable on the screen with the ability to rotate, scale and translate.
___
<img src="img/1.png" width="1400" height="800" alt="Main window"> 

## Main part

Developing a program to visualise the 3D wireframe models.

- The program developed in C++ language of C++17 standard
- The program code with MVC-pattern located in the src folder
- Writing code to follow the Google style
- The program built with Makefile which contains standard set of targets for GNU-programs: all, install, uninstall, clean, dvi, dist, tests
- The program developed according to the principles of object-oriented programming; the structured programming approach is not allowed
- Prepared full coverage of modules related to model loading and affine transformations with unit-tests
- There only one model on the screen at a time
- The program provides the ability to:
    - Load a wireframe model from an obj file (vertices and surfaces list support only).
    - Translate the model by a given distance in relation to the X, Y, Z axes.
    - Rotate the model by a given angle in relation to its X, Y, Z axes.
    - Scale the model by a given value.
- GUI implementation, based on any GUI library with API for C++ – **Qt**
- The graphical user interface contains:
    - A button to select the model file and a field to output its name.
    - A visualisation area for the wireframe model.
    - Button/buttons and input fields for translating the model.
    - Button/buttons and input fields for rotating the model.
    - Button/buttons and input fields for scaling the model.
    - Information about the uploaded model - file name, number of vertices and edges.
- The program correctly processes and allows user to view models with details up to 100, 1000, 10,000, 100,000, 1,000,000  vertices without freezing (a freeze is an interface inactivity of more than 0.5 seconds)
- The program implemented using the MVC pattern, and also:
    - there no business code in the view code
    - there no interface code in the controller and the model
    - controllers thin
- There at least three design patterns: facade, strategy and singleton

<img src="img/2.png" width="1400" height="800" alt="Settings">

## Settings

- The program allows customizing the type of projection (parallel and central)
- The program allows setting up the type (solid, dashed), color and thickness of the edges, display method (none, circle, square), color and size of the vertices
- The program allows choosing the background color
- Settings saved between program restarts

## Record

- The program allows saving the captured (rendered) images as bmp and jpeg files.
- The program allows recording small screencasts - the current custom affine transformation of the loaded object into gif-animation (640x480, 10fps, 5s) by a special button
- Thank you so much, @dbzhang800, for great record gif library https://github.com/dbzhang800/QtGifImage
 

 ___
 
<img src="img/3.GIF" width="800" height="600" alt="Gif"> 
