## 📜 About Project

**SAED** stands for Synopsys Armenia Educational Department, the university where I received my bachelor's degree. \
This project is course work that I have done during SAED's discrete mathematics course. \
The program finds a spanning tree in the user's inputted graph. \
For program-correct work, you must have [Graphviz](https://graphviz.org/) on your computer.

## 📶 Program Work Steps:

1. Get graph edges by reading the input file &nbsp;`input.txt`
2. Build an adjacency matrix for the given graph.
3. By using the adjacency matrix, make a simple graph from the given graph.
4. Check if the simple graph is connected or not, because a given graph must be connected.
5. If the graph is connected, find the spanning tree using the DFS algorithm.
6. Visualize the inputted graph and the spanning tree with Graphviz. \
[Input example](README_files/input_example.txt) &nbsp;&nbsp;&nbsp;&nbsp; [Output example](README_files/output_example.jpg)

## 👨‍💻 Getting Started

1. Start by updating the packages list: &nbsp;`sudo apt update`
2. Install G++ compiler, if you don't have: &nbsp;`sudo apt install build-essential`
3. Check installation with command: &nbsp;`g++ --version`
4. Make must be installed with build-essential package, check it: &nbsp;`make --version`
5. Install make package, if you don't have: &nbsp;`sudo apt install make`
6. Install Graphviz, if you don't have: &nbsp;`sudo apt install graphviz`
7. Check installation with command: &nbsp;`dot -V`
8. Clone this repo: &nbsp;`git clone https://github.com/dpetrosy/SAED_graph_project.git`
9. Go to directory: &nbsp;`cd graph_course_project`
10. Run make and build program: &nbsp;`make`
11. Run executable: &nbsp;`./graph.exe`

Congrats! Now you can see your inputted graph and found spanning tree :)
You can change `input.txt` file, and see how program works😎
