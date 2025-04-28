Vehicle Routing Problem (VRP) Solver Using Genetic Algorithm
This project solves a simplified Vehicle Routing Problem (VRP) using a Genetic Algorithm.
It optimizes routes for a set of vehicles to visit random locations with minimal total distance and balanced load among vehicles.

Features
Generates random delivery locations on a 2D plane.

Solves the VRP using a Genetic Algorithm (GA) with crossover, mutation, and selection strategies.

Ensures vehicles have balanced workloads using a balance penalty.

Visualizes the routes for each vehicle.

Technologies Used
Python 3.8+

NumPy

Matplotlib

DEAP (Distributed Evolutionary Algorithms in Python)

How to Clone and Run This Project in VS Code
1. Clone the repository
bash
Copy code
git clone https://github.com/your-username/vrp-genetic-algorithm.git
(Replace your-username with your GitHub username.)

2. Open the project in VS Code
Open VS Code.

Go to File > Open Folder and select the cloned project folder.

3. Install required libraries
Open a new terminal in VS Code and install the dependencies:

bash
Copy code
pip install numpy matplotlib deap
4. Run the project
Simply run the Python file (for example if your file is named main.py):

bash
Copy code
python main.py
If you are running from Jupyter Notebook or Google Colab, just execute the cells one by one.

How It Works
Random num_locations points are generated on a 2D plane.

num_vehicles vehicles are assigned to visit the locations.

A Genetic Algorithm evolves a population of candidate solutions:

Selection: Tournament selection chooses the best individuals.

Crossover: Partially matched crossover (PMX) exchanges parts of two solutions.

Mutation: Shuffle mutation randomly swaps points.

The fitness function minimizes:

Total distance traveled.

Balance penalty (ensuring all vehicles have similar workloads).

The best individual is visualized using a plotted route.

Usage
Each time you run the project, new random locations are generated.

The final plot shows the best routes for the vehicles starting and ending at the depot.

You can change:

num_locations to increase or decrease the number of delivery points.

num_vehicles to change the number of delivery vehicles.
