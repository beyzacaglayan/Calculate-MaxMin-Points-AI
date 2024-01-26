1-Genetic Algorithm
First, I defined import values in the Jupyter program. I chose the iteration value as 10, the maximum and minimum points as 1, and the pop_size as 9. So I initialized the population.
Then, I created the fun(x) function and wrote the required sine function.
I created a probability function. The probability value is obtained by dividing a fitness value by the total fitness value. I defined this in this function.
Then I wanted to create a population. According to the genetic algorithm, we need to assign random values to this population as fitness. I randomly selected the fitness_values and population 
values using epok.
Then I brought these values into elitism. Here, I assigned fitness until the pop_size value we defined at the beginning was equal to the population. I created an array from the population 
and fitness values and showed the epoch value. Here I constantly increased the epoch value and our final value became our final population value.
I selected the best value from our population array and the fitness value from our fitness values array.
Finally, we need to find the maximum and minimum values. To do this, I first had to show that the xMin and xMax values were in pop_size inside the population function.
Then I defined the xMin and xMax values inside the individual function because I want the minimum and maximum values to be individuals. Since it was necessary to randomly select these 
individuals, I directed the individual function to the random function and created a random function. This stage is the stage where we find the minimum and maximum values. If the number we 
randomly choose is less than the minimum value, we increase the number to the minimum so that we can find the smallest value. If the number we randomly choose is greater than the maximum, 
we increase the number up to the maximum so that we can find the maximum value in the same way.

2-Particle Swarm Optimization
First, I create a particle, that is, a list of particles, for the x value and create a function for this particle. Inside this function, I need to create a new particle for each iteration.
We will generate these particles randomly. For this, I created a list with new particles. To find the maximum and minimum values, I sorted this new list of particles from largest to smallest.
Afterwards, I had to define the speeds as the PSO algorithm asked us to. First of all, I created a speed function for the initial minimum and maximum speeds between -10,10 values. 
As I mentioned here, I defined that the first minimum and maximum speed between -10 and 10 should be returned.
I created separate functions for minimum and maximum speeds. In this function, I wrote the formulas specified in PSO optimization by specifying variables.
Afterwards, I created the functions (p_best_min, p_best_max) to create the best personal minimum and personal maximum values. Here we find the minimum and maximum points of the Personal 
Best value in the 3rd Step of the algorithm, as requested in the question. If f[i][a], f[i-1] is greater than [a], we return maximum, if it is smaller, we return minimum.
Likewise, we need to find the Global Best value, which is the next step in the algorithm. I created (g_best_min, g_best_max) functions to find the minimum and maximum points of these 
global best values. If f[a] is greater than g_best, we return the maximum, if it is smaller, we return the minimum.
Then, I created separate series for minimum and maximum values, global best values, minimum and maximum speeds, and personal best values. I added the value 0 to the minimum and 
maximum functions of the speeds. The first value of the personal best function will be x. I calculated the function before finding the personal best and global best values. Then I 
calculated and printed the minimum and maximum values of personal best, global best, speed and function.

![ai](https://github.com/beyzacaglayan/Calculate-MaxMin-Points-AI/assets/54523165/11d4d74a-a7fb-4934-8278-ec1c1badad56)
