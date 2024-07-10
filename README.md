# The Maze

The Maze is a 3D maze game that transforms a 2D map into a 3D navigable world using ray casting. Written in C with the SDL2 library, the project was developed on Ubuntu 14.04 LTS with gcc 4.8.4.

![Maze Screenshot](screenshots/maze.png)

## Inspiration and Story

The Maze project began as a fascination with the complexity and beauty of mazes. I wanted to create an immersive experience that combined my interest in algorithms and game development. The challenge was to build a visually engaging 3D maze game from a simple 2D map, which led me to explore the intricacies of ray casting and optimization techniques.

## Technical Challenge

The core technical challenge was to efficiently render a 3D maze from a 2D grid using ray casting. This involved understanding and implementing complex algorithms while managing performance and memory constraints. I chose the SDL2 library for its versatility in handling graphics, audio, and input across platforms.

### Key Features

- **Ray Casting**: Converts 2D maps into 3D worlds.
- **Optimized Algorithms**: Uses heuristic optimizations in A* and recursive backtracking for efficient maze generation and solving.
- **Interactive Navigation**: Allows movement and camera control within the 3D maze.

## Struggles and Learning

The journey was filled with unexpected challenges:

1. **Algorithm Complexity**: Initially underestimated the computational cost and memory usage of algorithms like A* and Dijkstra's.
2. **Edge Cases**: Handling multiple solutions, loops, and dead ends required robust validation.
3. **Integration**: Ensuring seamless communication between components was harder than anticipated.

Through perseverance and constant learning, I refined my approach, incorporated optimization techniques, and adopted a modular structure for better integration and testing.

## Vision for Next Iteration

For the next iteration, I envision:

- **Enhanced Visualization**: Adding interactive features like step-by-step solving visualization and user-defined maze parameters.
- **Automated Testing and CI**: Implementing comprehensive automated testing and setting up a continuous integration pipeline.
- **Graphical UI**: Upgrading the text-based interface to a graphical user interface (GUI) for a more immersive experience.

## Technical Depth

### Ray Casting

Ray casting is the backbone of rendering the 3D maze. It involves projecting rays from the player's viewpoint and calculating intersections with walls to create a 3D perspective.

### Maze Generation

I used recursive backtracking for maze generation, which is efficient and ensures a solvable maze with intricate pathways.

### A* Algorithm

For solving the maze, the A* algorithm was chosen for its efficiency and ability to incorporate heuristic optimizations, making it faster than other pathfinding algorithms like Dijkstra's.

## Installation

To get started, clone the repository:

```bash
$ git clone https://github.com/Pierre254/The-Maze-Project.git

Usage
$ gcc -Wall -Werror -Wextra -pedantic ./src/*.c -lm -o maze $(sdl2-config --cflags --libs)
$ ./maze
