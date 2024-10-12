## Solve the Travelling Salesman Problem to Find the Optimal Driving Route by Genetic Algorithm

### What is the Travelling Salesman Problem (TSP)?
Definition: *Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the initial city? (Gutin & Punnen, 2007)*

<img align="center" src="https://sketchplanations.com/_next/image?url=https%3A%2F%2Fimages.prismic.io%2Fsketchplanations%2F611d51e9-25b7-4d00-a800-ccde2e672a39_190464809359.jpg%3Fauto%3Dcompress%2Cformat&w=1080&q=75"> Source: https://sketchplanations.com/the-travelling-salesman-problem

The TSP is a combinatorial optimization problem, which has a high complexity and having a search space of n!. The following plot shows how the search space increases exponentially with the number of cities.

<img align="center" src="search_space.png">

Obviously, it's infeasible to use the brute-force method enumerating all combinations and compute their distances, as it may take too much computational time.

### Optimization Algorithms
In order to solve this problem, optimization algorithms can help us with finding the optimal solution. For the traditional approaches in solving the TSP, integer programming (Miller et al, 1960) and dynamic programming (Bellman, 1962) were proposed to solve the TSP by finding the exact solution. However, they fail to search for the exact solution within practical timeframe due to scalability.

Later, heuristic algorithms were developed to tackle larger instances of TSPs. They are algorithms that focus on local search mechanisms and design, which the nearest neighbor algorithm (Rosenkrantz et al., 1977) was a popular choice to solve optimization problems. Moreover, they aim to provide near-optimal solution instead of exact solution, but stuck in local optima when solving larger instances of TSPs.

Starting from the 2000s, methodologies of solving TSPs have been shifted towards metaheuristics, which are advanced heuristic algorithms to address scalability issue, with high efficiency. Unlike heurisitic algorithms, metaheurisitic does not require gradient information, which we don't need to have prior knowledge in the problem. And this is beneficial when dealing with lots of TSPs or complex optimization problems. Recently, various hybrid metaheurisitcs were proposed by combining different metaheurisitc algorithms to solve the TSP and other optimization problems. 

### Genetic Algorithm (GA)
The Genetic Algorithm is a nature-inspired metaheuristic algorithm which was proposed by Fraser (1957). GA was inspired by the evolutionary process of the nature. An image below shows how the human evolve through 6 million years. 
<img align="center" src="https://i0.wp.com/miro.medium.com/v2/resize:fit:1750/0*UambwL7iJjjEERaZ.jpg?ssl=1">
Source: https://i0.wp.com/miro.medium.com/v2/resize:fit:1750/0*UambwL7iJjjEERaZ.jpg?ssl=1

GA mimics some major mechanisms of evolutionary process, thus the main operations in the algorithm are "Selection", "Crossover", "Mutation". These operations may have different variants depending on the problem we are solving. The following section explains how GA works in solving TSP.

#### Initialization
#### Iterative Process
#### Selection
#### Crossover
#### Mutation


### File Description
- GA.ipynb is a document along with python codes, comments and markdowns of full explanation, as a notebook.
- 50_Landmarks.csv contains coordinates and addresses of the 50 waypoints.
- 50_Landmarks_Distance_Matrix.csv contains the 2500 distances data of the 50 waypoints.
- Best_route.html is an interactive map showing the driving route through 50 waypoints computed by GA.
