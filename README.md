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



  
