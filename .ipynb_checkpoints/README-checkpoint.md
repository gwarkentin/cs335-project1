# CPSC335 - Section 01 - Project 1: Greedy Approach to Hamilton Problem & Matching Group Schedules

### Gabriel Warkentin <gabrielwarkentin@csu.fullerton.edu>

[See assignment doc](./SP23_CPSC_335_Project 1_Description.pdf)


## Problem 1: Greedy Approach to Hamilton Problem

### 1.1) Problem Statement:

Cities in lie in a unidirectional circle, each city has limited fuel to give, distances between differ
Pick the 1 starting city which allows you to travel through all cities back to the start traveling clockwise.

Start with 0 gallons + the fuel of the first city

Sample Input:
city_distances = [5, 25, 15, 10, 15]
fuel = [1, 2, 1, 0, 3]
mpg = 10

The preferred starting city for the sample above is city 4

### 1.2) Solution Approach:

First thing is to determine what the net fuel per stop would be. It is most straightforward to build that into an array to analyze.

net_fuel[] = fuel[] * mpg - city_distances[]
fuel_tank = net_fuel[first_city]

Then, we can loop through each starting city, checking to ensure we don't run out of fuel (go negative) at any stop.

At worst, we will have through each city for each city, so that will be $O(n^2)


### 1.3) Pseudocode:





## Problem 2: Matching Group Schedules