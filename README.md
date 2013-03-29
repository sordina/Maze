# Maze

Generate a maze with the power of lenses!

Maze is output to STDOUT in [PBM](http://en.wikipedia.org/wiki/Netpbm_format) format.

<img src="https://raw.github.com/sordina/Maze/master/images/maze.png" alt="Example Maze" />

## Usage

    maze <width/2> <height/2> <entropy>*

The width and height of the maze are actually twice the number of pixels of the argument.
This is due to the minimum number of pixels required for a path including those of the walls.

Entropy refers to a repeating sequence of digits use for the cycled random seed.
If omitted, the built-in pseudo-random number generator will be used.

For example:

    maze 12 12 0
    maze 12 12 0 1
    maze 12 12 0 0 1
    maze 12 12 0 0 0 1
    maze 12 12 0 1 0 2 1

<img src="https://raw.github.com/sordina/Maze/master/images/maze_entropy.png" alt="Example Maze" />

## Example

Generate a random 6x6 maze, output to a pbm file, then convert to a png with [ImageMagick](http://www.imagemagick.org/script/index.php):

    maze 6 6 > maze.pbm
    convert maze.pbm maze.png
