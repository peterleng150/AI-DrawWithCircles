## AI-Draw

## What it does

The computer iteratively attempts to mimic an input pictures through drawing it with 300+ circles of varying circle and radii, and continuously improve its accuracy based on a generic genetic algorithm

## How I built it

I followed 3 main steps that are common in genetic algorithms:
1. Create population of a generation
2. Use the current generation to breed a new generation. More accurately drawn individuals will be more likely to pass its traits down to its children
3. Children will occasionally experience mutations, which are randomly occuring changes to their DNA properties.

In our case, the DNA would be the coordinates and colors of all our circles.

The actual app itself is built with the P5 JavaScript framework, which is similar to the Processing language/environment.

## Challenges I ran into
The most challenging aspect was trying to optimize our fitness function, our cross-breeding function, as well as our mutation function, as the simulation takes a long time, and usually it is very difficult to get significant results in an hour. Thus, I had to be very careful in terms of when to test.

In the end, I was not able to get a visibly optimal solution, but I believe that with further optimizations, the algorithm should be able to produce better results.

## How to install& run it 
```
git clone https://github.com/peterleng150/AI-Draw.git
cd AI-Draw
python -m SimpleHTTPServer
```
This should start a server on port 8000 on your local machine.

Created by Andrew Leng


