# Python Exercise: Modeling the Prisoner's Dilemma with Game Theory

## Problem Statement

In this exercise, you will be using Python to model the classic game theory problem known as the Prisoner's Dilemma. You will be using the Nashpy library to define the payoff matrix for the game and find the Nash Equilibrium, which represents the optimal strategy for each player.

## Instructions

1. **Setup your environment**: Install the necessary Python libraries. You will need Nashpy for this exercise. You can install it using pip:

    ```python
    pip install nashpy
    ```

2. **Define the payoff matrix**: The Prisoner's Dilemma is typically represented with a 2x2 matrix. Define this matrix in Python.

    ```python
    import numpy as np

    # Define the payoff matrix
    payoff_matrix = np.array([[[-1, -3]], [[-2, 0]]])
    ```

3. **Create the game**: Use the Nashpy library to create a game with the defined payoff matrix.

    ```python
    import nashpy as nash

    # Create the game
    game = nash.Game(payoff_matrix)
    ```

4. **Find the Nash Equilibrium**: Use the Nashpy library's function to find the Nash Equilibrium of the game.

    ```python
    # Find the Nash Equilibrium
    equilibria = game.support_enumeration()
    for eq in equilibria:
        print(eq)
    ```

5. **Interpret the results**: The Nash Equilibrium represents the optimal strategy for each player. Interpret the results and understand what they mean in the context of the Prisoner's Dilemma.

## Expected Outcome

By the end of this exercise, you should have a Python program that models the Prisoner's Dilemma and finds the optimal strategy for each player. You should understand how to use the Nashpy library to model game theory problems and find their Nash Equilibrium. You should also have a deeper understanding of the Prisoner's Dilemma and game theory in general.