### AI Laboratory work 2: Searching in Graphs

# The task description.

For this laboratory work you will have to impliment a couple of searching algorithms bases on the map of România.

# The map.csv file.
The map.csv file represents the relationship between the nodes (Romanian cities). This relationship have the following statesȘ
1. -1 - it can't be a road from a city to itself.
2. 0 - there is no road connecting the cities.
3. a positive value - the distance between this two cities.
The cvs. file is having the cities only on columns, the rows are in the same order of cities as columns.

# What should you implement:

You should implement all algorithms in the following list as separate functions, each in a separate file.
Each function should take at least the start and the destionation of the trip, with additional needed parameters and return the path of cities chosen by algorithm as a list.
The algorithms are:
* A-star.
* Breath first.
* Bidirectional Search.
* Depth first.
* Greedy best first search.
* Uniform Cost.

For the Greedy best first search you will also need this - the distance from each city to the Bucharest.
distance_Buharest= {"Arad":366, "Bucharest":0, "Craiova":160, "Drobita":242, "Eforie":161,
                    "Fagaras":176, "Giurgiu":77, "Hirsova":151, "Iasi":226, "Lugoj":244,
                    "Mehedia":241, "Neamt":234, "Oradea":380, "Pitesti":100, "RM":193,
                    "Sibiu":253, "Timisoara":329, "Urziceni":80, "Vaslui":199, "Zerind":374}