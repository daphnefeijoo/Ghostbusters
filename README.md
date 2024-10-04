This project centers around a unique twist on the classic Pacman game, where the objective is to locate scared, invisible ghosts using noisy sonar distance readings. As Pacman navigates the maze, blocks of color indicate potential ghost positions based on these readings, which are always non-negative and can vary by up to 7 units from the true distance. The project emphasizes implementing advanced inference techniques using Bayes Nets to refine ghost tracking beyond the default visual cues.

Key components of the project include:

Bayes Net Construction: Implementing the constructBayesNet function to create the framework necessary for inference.

Factor Operations: Developing the joinFactors function to combine probability factors and the eliminate function to simplify these factors by removing specific variables.

Exact Inference: Implementing inferenceByVariableElimination to address probabilistic queries, alongside methods for calculating observation probabilities and updating beliefs based on sensor readings through the observeUpdate and elapseTime methods in the ExactInference class.

Greedy Action Selection: Enhancing the GreedyBustersAgent to utilize belief distributions to choose actions that minimize distance to the closest ghost.

Particle Filtering: Implementing particle filtering techniques to track a single ghost by initializing a uniform distribution of particles, updating beliefs based on observations, and managing particle transitions over time.

By combining these methods, the project challenges students to effectively leverage probabilistic reasoning and inference algorithms, enabling Pacman to intelligently hunt ghosts based on the uncertain information provided by his sonar.



