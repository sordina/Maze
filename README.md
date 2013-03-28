# Maze

Generate a maze with the power of lenses!

Maze is output to STDOUT in [PBM](http://en.wikipedia.org/wiki/Netpbm_format) format.

<img src="https://raw.github.com/sordina/Maze/master/images/maze.png" alt="Example Maze" />

## Example

Generate a random 6x6 maze, output to a pbm file, then convert to a png with ImageMagick:

    maze 6 6 > maze.pbm
    convert maze.pbm maze.png
