cmake_minimum_required(VERSION 3.21)
project(MazeGenerator C)

add_executable(maze_generator
    src/bitmap.c
    src/dynamic_array.c
    src/model.c
    src/prims_maze.c
    src/renderer.c
    src/maze.c
)

target_compile_options(maze_generator
    PRIVATE
        -Wall
        -Werror
        -std=c17
        -pedantic
)
