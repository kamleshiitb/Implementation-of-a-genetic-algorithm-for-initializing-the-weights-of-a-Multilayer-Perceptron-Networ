# Implementation of a genetic algorithm for initializing the weights of a Multilayer Perceptron-Network

Genetic Algorithm (GA) is a search-based optimization technique based on the principles of Genetics and Natural Selection. It is frequently used to find optimal or near-optimal solutions to difficult problems which otherwise would take a lifetime to solve. It is frequently used to solve optimization problems, in research, and in machine learning.

#How do they work?
A set of random weights are generated. This is the neural network of the first agent. A set of tests are performed on the agent. The agent receives a score based on the tests. Repeat this several times to create a population.Select the top 10% of the population to be available to crossover. Two random parents are chosen from the top 10% and their weights are crossover. Every time a crossover occurs, there is a small chance of mutation: That is a random value that is in neither of the parent’s weights.
This process slowly optimizes the agent’s performance, as the agents slowly adapt to the environment.
