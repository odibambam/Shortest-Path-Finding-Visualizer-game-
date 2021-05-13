# Shortest-Path-Finding-Visualizer-game-
Used BFS algortihm to solve the problem of finding the shortest path from one point to another.

There are 4 Test cases for my project :
No Solution found
Diagonal Movement
Maze
Random undefined Maze

EXPLANATION OF CODE IS GIVEN BELOW :


Importing the following :
 Pygame (It imports all the available pygame modules into the pygame package).
Sys(It lets us access system-specific parameters and functions).
Math(To use mathematical functions).
random(returns an integer number selected element from the specified range).
Messagebox from tkinter (for great GUI).
Size of output box (graph) is 640 x 480.
Display.set_caption() for showing “Shortest Path Finding visualizer” on top of output box.
Starting point is 64th square position & ending point is 48th square position.

pygame.draw.rect() - This function is used to draw a rectangle.

Self.visited = false
Self.wall = false
Self.prev = none
False as we have not visited any node yet and not created any walls

// - floor division
W – width // cols
H – height // rows

def add.neighbors() – helps us explore neighboring nodes.

grid[i][j].add_neighbors(grid) - Is an easy way of finding the neighbours in a two-dimensional array.

Lines 81-87 - To check if there is any path from top left to bottom right.

A flag in Python acts as a signal to the program to determine whether or not the program as a whole or a specific section of the program should run.
In other words, you can set the flag to True and the program will run continuously until any type of event makes it False. Then the program, loop, or whatever you're using a flag for will stop.
clickWall – to create wall.
pygame.mouse.get_pressed – helps the compiler know when & where mouse is clicked i.e get the state of the mouse buttons.
Sys.exit() - function allows the developer to exit python.
pygame.MOUSEBUTTONUP - event occurs once when the mouse button is released.
pygame.K_RETURN – when enter key is pressed, exploration starts.
pygame.KEYDOWN - to detect if a key is physically pressed down or released.

If length of our queue is not 0, then we pop(remove) the leftmost element in the queue using current variable.
If we have found the point, our exploration / traversal should end.
If not then, we will continue exploring other nodes until we reach our desired node aka end point.
path.append() is a built-in function of sys module that can be used with path variable to add a specific path for interpreter to search.
The tkinter package (“Tk interface”) is the standard Python interface to the Tk GUI toolkit.
Wm.withdraw() - Withdraws the widget from the screen such that it is unmapped and forgotten by the window manager.
If we do not reach / find our end point (noflag condition) then the compiler will display “Shortest Path Finding Visualizer” on top of the message output box and give a pop-up “There was no Solution” using messagebox.showinfo() 

Win.fill() is used to display the colour of our exploration.
Colour codes :
(255,255,255) - White 
(25,120,250) - Green
(255,0,0) - Red 
(0,120,255) - Blue 
Spot.show(win,(255,255,255)) displays white colour as this area is still unexplored.
Spot.show(win,(25,120,250)) displays green colour as we are still exploring.
Spot.show(win,(0,120,255)) displays blue colour joining the start node/point and end point/node.
Spot.show(win,(255,0,0)) displays red colour entirely alongside the blue path. Once, we have reached the desired node.  
pygame.display.flip() will update the contents of the entire display.
