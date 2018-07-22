# Optimization-with-Genetic-Algorithms
Implementation of  a genetic algorithm (GA) for  the clustering of the nodes of a graph. Done for the Neural and Evolutionary Computation subject.

### Exercise statement

#### Objective
Implementation of a genetic algorithm(GA) for the clustering of the nodes of a graph, by means of the optimization of modularity.

#### Modularity
![Modularity](https://raw.githubusercontent.com/franfj/Optimization-with-Genetic-Algorithms/master/modularity.png)

#### Genetic algorithm
Given the network G, any vector S may be seen as the chromosome corresponding to a partition in two clusters, and the fitness is related to its modularity Q(S).

The objective is the  implementation  of  a  genetic  algorithm to  obtain  the  partition which  maximizes modularity.

#### Fitness
Modularity cannot be used directly as the fitness since it may take negative values, and also the difference in modularity of good partitions may be very small. You should define a transformation of modularity into an adequate positivefitness function, use the rank, or try with robust selection methods.

#### Data
- Input: a network in Pajek format (*.net | More info in http://pajek.imfm.si/)
- Output: the highest modularity partition found, in Pajek format (*.clu), and its corresponding value of modularity

#### Parameters
Try different variants of the genetic algorithm and of their corresponding parameters, for instance:
- Fitness function
- Selection schemes: proportional (roulette-wheel), truncation, ranking, tournament, fitness uniform (FUSS), etc.
- Crossover: one-point crossover, two-point crossover, uniform crossover, etc.
- Mutation
- Elitism

#### Example
This is the “real” partition of the Zachary Karate Club network, as a reference for a good partition in two communities (not necessarily the one with largest modularity).

![Example](https://raw.githubusercontent.com/franfj/Optimization-with-Genetic-Algorithms/master/example.png)
