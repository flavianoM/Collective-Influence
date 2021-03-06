Created in 2016

Author: Flaviano Morone

# Collective-Influence
Collective Influence Algorithm to find influencers in complex networks

To compile the source code use the command

gcc -o CIA CIA.c -lm -O3 

To run the executable use the command:

./CIA NETWORK_FILENAME R

where - NETWORK_FILENAME - is the file containing the network and - R - is an integer defining the radius of the Influence's Sphere. 

The data structure in the file - NETWORK_FILENAME - must be formatted as an adjacency list of the following type:


node_1 first_neigh_of_node_1 second_neigh_of_node_1 ... last_neigh_of_node_1
node_2 first_neigh_of_node_2 second_neigh_of_node_2 ... last_neigh_of_node_2
...... ..................... ...................... ... ....................
node_N first_neigh_of_node_N second_neigh_of_node_N ... last_neigh_of_node_N


In each line of the adjancency list the first number is the node_ID and the following numbers are the ID's of the its neighbors.

At output, the program prints at screen the values of (q,G), where q is the fraction of removed nodes and G is the size of the giant component of the graph. 
Also, the program creates a file "Influencers.txt" with a list of the influencers in the network, ordered by decreasing influence.  



For more information, visit https://www.nature.com/articles/nature14604  
  
