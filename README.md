Download Link: https://assignmentchef.com/product/solved-csci-3104-assignment-7
<br>
<ol>

 <li>(100 points) For this assignment, you will implement simple map routing using different algorithms. First, we will be dealing with geographic vertices, in a simplified way. These vertices are points in the 2D plane (with <em>x </em>and <em>y </em>coordinates) connected by edges which are Euclidean distances. For simplicity, you may assume that 0 <em>&lt; x,y &lt; </em>

  <ol>

   <li>For the first part, you will read in a graph from a text file. The text file will contain (1) the number of vertices and edges, (2) the numbered vertices along with their respective <em>x </em>and <em>y </em>coordinates, (3) the edges represented as pairs of vertices. Additionally, for testing, the source and destination vertices will be included. As an example, we could represent the following graph as a text file (Note: the last line represents source and destination vertex, i.e. we want to search from vertex 2 to 1):</li>

  </ol></li>

</ol>

1

6 9

<ul>

 <li>250 500</li>

 <li>1700 200</li>

 <li>800 900</li>

 <li>1200 600</li>

 <li>400 200</li>

 <li>900 100</li>

</ul>

0 1

<ul>

 <li>2</li>

 <li>3</li>

 <li>3</li>

</ul>

2 4

<ul>

 <li>5</li>

 <li>4</li>

 <li>5</li>

 <li>5</li>

</ul>

2 1

You can choose to represent the graph any way you like (e.g. an adjacency list).

<ol>

 <li>Next, you must implement code to check whether the input graph contains a cycle.</li>

 <li>In addition, you need to implement two shortest-path algorithms: (1) the algorithm we discussed in class for DAGs, and (2) Dijkstra’s algorithm. Based on the result of the cycle check routine, you need to call your DAG shortest-path algorithm if the input graph is acyclic, or your Dijkstra algorithm if it contains a cycle. The output of either of these routines is (1) The source and destination vertex, (2) the total distance of the shortest path between them, and (3) the actual sequence of vertices that form the shortest path, in the correct order.</li>

 <li>Finally, you must implement code that will plot the shortest path found by your shortest-path algorithm(s), along with the Euclidean distances between vertices on this path.</li>

</ol>

<strong>Note: </strong>All of your implementations must run efficiently, e.g. the DAG shortest-path algorithm should run in O(<em>V </em>+<em>E</em>). Provide evidence (plots) that show your implementations are sufficiently fast.

<ol start="2">

 <li><strong>Extra Credit: (10 points) </strong>Optimize Dijkstra’s algorithm so that once you have read in your graph, any shortest-path search takes sublinear time. Note that you are not allowed to simply compute and store all shortest-paths for all pairs of vertices, i.e. assume you cannot afford the space requirement for doing so. You must clearly show that your optimizations meet the time complexity criteria.</li>

</ol>

2