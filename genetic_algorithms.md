## CS 344 Honors Project - GA Background Information
###### Elizabeth Koning
###### March 18, 2019
####

### Source 1: Wikipedia
https://en.wikipedia.org/wiki/Genetic_algorithm

definition: metaheuristic inspired by the process of natural selection

It will involve things like mutation, crossover, and selection.

- Methodology
  - Optimization problems
    - population of candidate solutions is evolved towards better solutions
    - Start with randomly generated individuals
    - Uses all the biology words
    - Evaluates the fitness for each individual in the generation
    - Select the more fit individuals and use recombination and random mutation for the next generation
    - terminates after maximum number of generations or satisfactory fitness in population
    - Requires:
      - genetic representation of domain
      - fitness function to evaluate solution
    - typically represented with an array of bits
      - good for simple crossover operations
  - Initialization
    - starts with hundreds or thousands of possible solutions
    - can be seeded for more likely areas of solutions, but often random
  - Selection
    - Separate article for more detail
    - "fittest" are selected to breed new generation
    - measures the quality of represented solution
      - knapsack problem: fitness = sum of values of all objects if representation is valid, or 0 if it is not valid
      - can be quite difficult to measure
  - Genetic operators
    - Crossover and Mutation have their own articles
    - parent solutions are selected for breeding - use crossover and mutation to create new solution with shared characteristics
    - can use more than two parents, sometimes gives higher quality chromosomes
    - tune parameters: mutation probability, crossover probability, and population size make a difference
  - Heuristics
    - speciation - can penalize crossover between similar candidate solutions
  - Termination
    - many options - satisfy criteria, max number of generations, allocated time reached, ...
- The building block hypothesis
- Limitiations
  - fitness function evaluation can be prohibitive
  - do not scale well with complexity
  - "better" is comparitive, so stop criterion is not always clear
  - local optima rather than global
    - can be alleviated by increasing mutation rate
    - can use "niche penalty" where too similar of individuals are penalized
    - dynamic data sets is difficult - converge early and may not be valid later
    - only works if there is a hill to climb, not binary measure
    - other algorithms may be more efficient
- Variants
  - To be read at a later date if it becomes relevant
- Problem domains
  - timetabling and scheduling problems are particular fitting
  - engineering
  - global optimization problems
  - complex fitness landscape - move away from local optima better than traditional hill climbing
- More sections with less relevance, including history

### Source 2: MathWorks
https://www.mathworks.com/help/gads/what-is-the-genetic-algorithm.html

This source is less helpful than the Wikipedia article, but may become more helpful if I am interested in their implementations.
