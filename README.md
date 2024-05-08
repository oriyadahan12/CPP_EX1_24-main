t"g oriyati0701@gmail.com | 327510616

# SYSTEM PROGRAMMING 2- ASSIGNMENT 1

My code deals with graphs and looking at all kinds of features in the graph.
We represent the matrix in an adjacency matrix in which the weight of the edges it has with the other vertices is written for each vertex (if it doesn't have a common edge, the matrix has a value of 0).
I built some methods for extracting information and data from the graph we will receive.
And I'll start with an explanation of loading a graph into a matrix:

 the loading-graph function:
 
    /* @brief Initializes the graph with the provided adjacency matrix.
    * 
    * This function initializes the graph's adjacency matrix with the provided matrix.
    * It checks if the matrix is square and throws an invalid_argument exception if not.
    * It also checks if there is any vertex with an edge to itself and throws an exception if found.
    * 
    * @param adjacencyMatrix The adjacency matrix representing the graph.
    * @throw std::invalid_argument If the matrix is not square or if there is a vertex with an edge to itself.
    */
     void ariel::Graph::loadGraph(vector<vector<int>>adjacencyMatrix){}

After loading the graph into our matrix, we can start running the methods.
We will start with simple functions such as printing the graph and finding the number of vertices in the graph.

The print function:

    /*
    * @brief Prints information about the graph.
    * 
    * This function prints the number of vertices and edges in the graph.
    */
       void ariel::Graph::printGraph(){}


 The function that find the number of vertex in the graph:

    /**
        * @brief Returns the number of vertices in the graph.
        * 
        * @return The number of vertices in the graph.
        */
       size_t countVer();

 Now we will continue with the functions with the more complex algorithms that I wrote:

I will start by detailing my privacy functions.

Bellman-Ford function:
Goes through all the edges n-1 times and makes a placement for each edge on the minimum weight that can be reached in it.
The function can work with negative weights and find negative circles in the graph (if they exist).

     /**
     * @brief Applies the Bellman-Ford algorithm to find the shortest paths from a given start vertex.
     * 
     * This function computes shortest paths from the start vertex to all other vertices in the graph using the Bellman-Ford algorithm.
     * It updates the input vectors 'd' and 'pi' to store the shortest distances and predecessors respectively.
     * 
     * @param g The graph on which to perform the algorithm.
     * @param start The index of the starting vertex.
     * @param d Vector to store the distances from the start vertex to each other vertex.
     * @param pi Vector to store the predecessors of each vertex in the shortest paths.
     */
    static void bellmanFord(Graph g, size_t start, std::vector<int>& d, std::vector<int>& pi);
  
Another function we will use later is the DFS function.
This is a deep search function that goes over a vertex and all its children and colors the vertices in several different colors according to their current state (whether we are done with them or not, etc.)

We used this function to find circles in the graph.


  
