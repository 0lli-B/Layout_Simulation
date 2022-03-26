# Layout_Simulation
Exercise: optimizing a machine layout in a new production hall (greenfield construction).<br>
Size of the hall: 5x5 units of length (1 unit == 3 meters); place is completely free (no obstacles)<br>
1 fix raw parts warehouse, 1 fix finished parts warehouse, 5 machines to be placed (each with a size of 1x1 units).<br>
5 different products will be produced on these machines, each with a different processing order through the machines.<br>
Based on the production plan the number of products for the next period is given & the material flow matrix was calculated.<br>
# Program:
The simulation results will be written to an excel file; if it allready exits, the new simulation results will be appended.<br>
The simulation is programmed object oriented, a class for the machines and the two warehouses was created.<br>
For the layout another class was created, which is initialized with a random layout.<br>
The warehouses spawn at the same exact place, after that the 5 machines spawn random (they respawn if they are on a used place)<br>
The machines have a given color to be distinguishable.<br>
