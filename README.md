# Implementation of Genetic Algorithm (GA) and test its functionality on arbitary test functions.
About GA: GA works with a binary representation of solutions to the optimization problem and uses elitism, crossover and random mutation to produce better solutions for next generations. GA (with specific settings for this assignment - population size, elitism, selection process, mutation probability, stopping criterion)

## Randomly generate first generation (G = 1) of 50 solutions and evaluate their quality by an objective function
- While generation number G <= 1000, G++
- Move best 20% of the population (10 individuals) into the next generation, 20x
- Use rank/roulette selection mechanism to select 2 mutually different parents
- One-point crossover of parents to produce 2 children binary vectors
- Mutate (bit-flip) each bit of children vectors with a probability of 1%
- Evaluate the quality of children vectors and place them into the next generation
- The next generation should be complete with 50 individuals (best 10 from the previous generation, 40 new children)
- Store the best-found solution as the result (Also keep the best solution from every generation to produce a convergence graph)
- If the best-found solution is optimal, stop the loop.
- Return the best-found solution

## Evaluation
- Use GA on each test function (you should have 5 of them) with the 50D dimensionality (bit strings of length 50), run it 30x and find the best, worst, average and median solution quality and the standard deviation.
- Plot the convergence plots for each function and all 30 runs.
- Show the average convergence plot for each function.

## Extra
- Test functions in 10D, 30D, and 100D - adjust the number of generations and population size accordingly
