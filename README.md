Overview
The code consists of two main parts:

Simulation Functions: These functions handle the simulation of the game. They include functionalities to deal cards, determine scores, simulate player actions, and evaluate the game outcome.

Monte Carlo Control: This part employs Monte Carlo methods to find an optimal policy for playing Blackjack. It iteratively updates the action-value function to improve the policy over time.

How to Use
To run the simulation and obtain the optimal policy:

Ensure you have Julia installed on your system.

Copy the provided code into a Julia environment or script file.

Execute the code. This will run the Monte Carlo control algorithm to find the optimal policy for playing Blackjack.

After execution, the code will generate heatmaps illustrating the optimal policy for different game scenarios.

Components
Simulation Functions
deal_cards(n): Simulates dealing n cards from a shuffled deck.
usable_ace(hand): Determines if an ace in the hand can be used as 11 without busting the hand.
score(hand): Calculates the score of a given hand.
blackjack(π, ϵ): Simulates an episode of Blackjack according to a given policy π. It also handles player actions and determines the game outcome.
MC!(q, qn, π): Implements the Monte Carlo control algorithm to find the optimal policy. It iteratively updates the action-value function q based on observed rewards.
Monte Carlo Control
π: Initial policy for playing Blackjack.
q: Action-value function representing the expected return for each state-action pair.
qn: Holds the number of observations for each state-action pair during Monte Carlo updates.
MC!(q, qn, π): Monte Carlo algorithm for finding the optimal policy.
Visualization
The code provides visualizations in the form of heatmaps to illustrate the optimal policy for playing Blackjack under different scenarios.

Note
This code aims to find an optimal policy for playing Blackjack using Monte Carlo control.
The provided functions are tailored for a simplified version of Blackjack and may not cover all edge cases or variations of the game.
Adjustments or extensions may be necessary for specific applications or variations of the game.
Feel free to explore and modify the code according to your requirements or use case.

Disclaimer: This code is intended for educational purposes only. It may not be suitable for real-world applications without further validation and modifications.
