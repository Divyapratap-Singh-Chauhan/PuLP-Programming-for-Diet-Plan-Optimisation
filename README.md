# Diet Plan Optimization using PuLP

## Overview

This project demonstrates how to use linear programming to create an optimized diet plan using the PuLP library in Python. The goal is to minimize the cost of the diet while meeting the nutritional requirements for a balanced diet. This is a classic linear programming problem known as the "Diet Problem."

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Getting Started](#getting-started)
- [Problem Statement](#problem-statement)
- [Solution Approach](#solution-approach)
- [Results](#results)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

Linear programming is a powerful mathematical technique for optimizing a linear objective function, subject to linear equality and inequality constraints. This project applies linear programming to optimize a diet plan, ensuring that nutritional requirements are met at the lowest possible cost.

## Project Structure

The project directory is organized as follows:

```
Diet-Plan-Optimisation-using-PuLP/
│
├── data/
│   └── food_data.csv              # Dataset containing nutritional information of various food items
│
├── diet_plan_optimization.py      # Main Python script for optimization
│
├── results/
│   └── optimal_diet_plan.csv      # Output file containing the optimized diet plan
│
└── README.md                      # Project README file
```

## Dependencies

This project requires the following Python libraries:

- `PuLP` - A Python library for linear programming
- `Pandas` - For data manipulation and analysis

You can install the required libraries using the following command:

```bash
pip install pulp pandas
```

## Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Divyapratap-Singh-Chauhan/Diet-Plan-Optimisation-using-PuLP-Linear-Programming---Optimisation.git
   cd Diet-Plan-Optimisation-using-PuLP-Linear-Programming---Optimisation
   ```

2. **Prepare the dataset:**

   The `food_data.csv` file in the `data/` directory contains the nutritional information for various food items. Ensure that this file is present and correctly formatted.

3. **Run the optimization script:**

   Execute the main script to generate the optimized diet plan:

   ```bash
   python diet_plan_optimization.py
   ```

4. **View the results:**

   The optimized diet plan will be saved in the `results/` directory as `optimal_diet_plan.csv`.

## Problem Statement

The diet problem aims to select a combination of foods that meet all nutritional requirements at the minimum cost. The specific requirements include:

- **Calories**
- **Protein**
- **Fat**
- **Carbohydrates**
- **Vitamins and Minerals**

Each food item in the dataset has associated nutritional values and costs. The objective is to minimize the total cost while satisfying the nutritional constraints.

## Solution Approach

### 1. **Data Preparation:**

   The dataset is loaded and processed to extract relevant nutritional information and costs.

### 2. **Formulating the Linear Program:**

   The problem is formulated as a linear program, where:
   
   - **Objective Function:** Minimize the total cost of the selected food items.
   - **Constraints:** Ensure that the selected food items meet or exceed the daily nutritional requirements.

### 3. **Solving the Linear Program:**

   The PuLP library is used to define and solve the linear program. The solver finds the optimal combination of food items that minimize the cost while satisfying the constraints.

### 4. **Generating the Output:**

   The optimized diet plan, including the quantities of each selected food item, is saved as a CSV file.

## Results

The optimized diet plan is generated and saved in the `results/optimal_diet_plan.csv` file. This file contains the list of food items, their respective quantities, and the total cost of the diet plan.

## Conclusion

This project demonstrates how linear programming can be applied to real-world problems such as diet optimization. By leveraging the PuLP library, we were able to create an optimized diet plan that minimizes cost while meeting all nutritional requirements.

## References

- [PuLP Documentation](https://coin-or.github.io/pulp/)
- [Linear Programming and Optimization Overview](https://en.wikipedia.org/wiki/Linear_programming)
- [The Diet Problem](https://www.math.utah.edu/~gustafso/s2015/2270/projects/diet_problem.pdf)
