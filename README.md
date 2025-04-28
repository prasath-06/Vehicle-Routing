Vehicle Routing Problem (VRP) Solver Using Genetic Algorithm:

This project solves a simplified Vehicle Routing Problem (VRP) using a Genetic Algorithm.
It optimizes routes for a set of vehicles to visit random locations with minimal total distance and balanced load among vehicles.

Features:
1. Generates random delivery locations on a 2D plane.
2. Solves the VRP using a Genetic Algorithm (GA) with crossover, mutation, and selection strategies.
3. Ensures vehicles have balanced workloads using a balance penalty.
4. Visualizes the routes for each vehicle.

Technologies Used:
1. Python 3.8+
2. NumPy
3. Matplotlib
4.DEAP (Distributed Evolutionary Algorithms in Python)

How to Clone and Run This Project in VS Code:
1. Clone the repository:
git clone https://github.com/your-username/vrp-genetic-algorithm.git
(Replace your-username with your GitHub username.)

2. Open the project in VS Code
Open VS Code.
Go to File > Open Folder and select the cloned project folder.

3. Install required libraries
Open a new terminal in VS Code and install the dependencies:
pip install numpy matplotlib deap

5. Run the project
Simply run the Python file (for example if your file is named main.py):
python main.py

How It Works
1. Random num_locations points are generated on a 2D plane.
2. num_vehicles vehicles are assigned to visit the locations.
  A Genetic Algorithm evolves a population of candidate solutions:
    1. Selection: Tournament selection chooses the best individuals.
    2. Crossover: Partially matched crossover (PMX) exchanges parts of two solutions.
    3. Mutation: Shuffle mutation randomly swaps points.
  The fitness function minimizes:
    1. Total distance traveled.
    2. Balance penalty (ensuring all vehicles have similar workloads).


Usage
Each time you run the project, new random locations are generated.
The final plot shows the best routes for the vehicles starting and ending at the depot.


