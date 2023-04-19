# FPGA_final_subway

use vivado to synthesis and implementation

## RTL Design desciption
A circuit to play Subway Surfers.

The straight line map is a 4*64 matrix.The character can only move on this map. The player will see different types of objects on the tracks. 

The player need to run forward and dodge the obstacles by straight forward, swiping left, swiping right, and jumping in order to avoid them.

The pattern will send the initioal position of the character in the beginning of the game. The objects in the map have 4 types(2-bits):road(2'b00),lower obstackes(2'b01),higher obstacles(2'b10),tarins(2'b11).

The 2-bit inputs for 4 tracks (in0, in1, in2, in3) is given 64 cycles continuously. For simplicity, hugher and lower obstacles and trains can only be randomly generated in specific regions.
