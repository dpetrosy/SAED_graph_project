## 📜 About Project

**SAED** stands for Synopsys Armenia Educational Department, the university where I received my bachelor's degree. \
This project is course work that I have done during SAED's discrete mathematics course. \
The program finds a spanning tree in the user's inputted graph. \
For program-correct work, you must have [Graphviz](https://graphviz.org/) on your computer.

## 📶 Program Work Steps:

1. Get graph edges by reading the input file &nbsp;**<code>input.txt</code>**
2. Build an adjacency matrix for the given graph.
3. By using the adjacency matrix, make a simple graph from the given graph.
4. Check if the simple graph is connected or not, because a given graph must be connected.
5. If the graph is connected, find the spanning tree using the DFS algorithm.
6. Visualize the inputted graph and the spanning tree with Graphviz. \
[Input example](README_files/input_example.txt) &nbsp;&nbsp;&nbsp;&nbsp; [Output example](README_files/output_example.jpg)

## 👨‍💻 Getting Started
#### 1. Start by updating the packages list: &nbsp;**<code>sudo apt update</code>**
#### 2. Install G++ compiler, if you don't have: &nbsp;**<code>sudo apt install build-essential</code>**
#### 3. Check installation with command: &nbsp;**<code>g++ --version</code>**
#### 4. Make must install with build-essential package, check it: &nbsp;**<code>make --version</code>**
#### 5. Install make package, if you don't have: &nbsp;**<code>sudo apt install make</code>**
#### 6. Install graphviz, if you don't have: &nbsp;**<code>sudo apt install graphviz</code>**
#### 7. Check installation with command: &nbsp;**<code>dot -V</code>**
#### 8. Clone this repo: &nbsp;**<code>git clone https://github.com/dpetrosy/graph_course_project.git</code>**
#### 9. Go to directory: &nbsp;**<code>cd graph_course_project/code</code>**
#### 10. Run make and build program: &nbsp;**<code>make</code>**
#### 11. Run executable: &nbsp;**<code>./graph.exe</code>**
#### Congrats! Now you can see your inputted graph and found spanning tree :)
#### You can change **<code>input.txt</code>** file, and see how program works😎
