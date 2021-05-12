# Implementation of a genetic algorithm for initializing the weights of a Multilayer Perceptron-Network

Genetic Algorithm (GA) is a search-based optimization technique based on the principles of Genetics and Natural Selection. It is frequently used to find optimal or near-optimal solutions to difficult problems which otherwise would take a lifetime to solve. It is frequently used to solve optimization problems, in research, and in machine learning.

# How do they work?

A set of random weights are generated. This is the neural network of the first agent. A set of tests are performed on the agent. The agent receives a score based on the tests. Repeat this several times to create a population.Select the top 10% of the population to be available to crossover. Two random parents are chosen from the top 10% and their weights are crossover. Every time a crossover occurs, there is a small chance of mutation: That is a random value that is in neither of the parent’s weights.
This process slowly optimizes the agent’s performance, as the agents slowly adapt to the environment.

# Genetic algorithm works in 5 phases
# 1. Initial population
This step starts with guessing of initial sets of a and b values which may or may not include the optimal values. These sets of values are called as ‘chromosomes’ and the step is called ‘initialize population’. Here population means sets of a and b [a,b]. Random uniform function is used to generate initial values of a and b. In this optimization problem, six sets of a and b values are generated between 1 and 10.

# 2. Fitness function
In this step, the value of the objective function for each chromosome is computed. The value of the objective function is also called fitness value. This step is very important and is called ‘selection’ because fittest chromosomes are selected from the population for subsequent operations.

# 3. Selection
Based on the fitness values, more suitable chromosomes who have possibilities of producing low values of fitness function (because the value of our objective function needs to be 0) are selected and allowed to survive in succeeding generations. Some chromosomes are discarded to be unsuitable to produce low fitness values.

# 4. Crossover
This step is called ‘crossover’. In this step, chromosomes are expressed in terms of genes. This can be done by converting the values of a and b into binary strings which means the values need to be expressed in terms of 0 or 1.

# 5. Mutation
his step is called ‘mutation’. Mutation is the process of altering the value of gene i.e to replace the value 1 with 0 and vice-versa. For example, if offspring chromosome is [1,0,0,1], after mutation it becomes [1,1,0,1]. Here, 2nd value of the offspring chromosome is decided to get mutated. It has got changed to 1 from 0.

# Data collection and Training the model
We have used MNIST Dataset in our project to train the Multilayer perceptron network.The MNIST database (Modified National Institute of Standards and Technology database) is a large database of handwritten digits that is commonly used for training various image processing systems. The database is also widely used for training and testing in the field of machine learning. It was created by "re-mixing" the samples from NIST's original datasets. The creators felt that since NIST's training dataset was taken from American Census Bureau employees, while the testing dataset was taken from American high school students, it was not well-suited for machine learning experiments. Furthermore, the black and white images from NIST were normalized to fit into a 28x28 pixel bounding box and anti-aliased, which introduced grayscale levels.

# Advantages and Disadvantages:
# Advantages:
1. Computationally not intensive
There are no linear algebra calculations to be done. The only machine learning calculations necessary are forward passes through the neural networks. Because of this, the system requirements are very broad, as compared to Deep Neural Networks.
2. Adaptable
One could adapt and insert many different tests and ways to manipulate the flexible nature of genetic algorithms. One could create a GAN within a Genetic algorithm, by making the agents propagate Generator networks, and the tests being the discriminators. This is a critical benefit, that persuades me that the use of genetic algorithm will be more widespread in the future.
3. Understandable
For normal neural networks, the learning patterns of the algorithm are enigmatic at best. For genetic algorithms it is easy to understand why some things come about: For example, when a genetic algorithm is given the Tic-Tac-Toe environment, certain recognizable strategies slowly develop. This is a large benefit, as the use of machine learning is to use technology to help us gain insight on important matters.

# Disadvantages:
Takes a long period of time
Unlucky crossovers and Mutations could result in a negative effect on the program’s accuracy, and therefore make the program slower to converge or reach a certain loss threshold.

#Methodology for Initialization of weights for Neural Network
