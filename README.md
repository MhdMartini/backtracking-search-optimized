# backtracking_search_optimized

This is an improvement over the baseline backtracking search algorithm which I implemented in my backtracking_search_maze_gen repo.
Instead of backtracking every step taken to get to the next searchable cell, the agent finds the shortest path to the searchable cell, using the Flood Fill algorithm. Agent search is still UNINFORMED, as agent only uses the previously visited cells to calculate the shortest path.


Generate a random maze:
    python maze_gen.py [--width WIDTH] [--help | -h]

        --width:    width of square maze, default is 75


Search a map:
    python searcher.py [--map MAP] [--start START] [--vid VID] [--help | -h]

        --map:      path to map image, default is maps/map2_100_i.png
        --start:    start position <row,col>, default is randomly generated
        --vid:      boolean for video output, default is False
