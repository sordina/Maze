# Maze

Generate a maze with the power of lenses!

## Example

Generate a random 6x6 maze, output to a pbm file, then convert to a png with ImageMagick:

    do maze 6 6 > maze.pbm
    convert maze.pbm maze.png
