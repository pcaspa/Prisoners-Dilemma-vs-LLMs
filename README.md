# Prisoners Dilemma vs Large Language Models

This code simulates various strategies in the Prisoner's Dilemma game, a classic example of game theory that illustrates why two completely rational individuals might not cooperate, even if it appears that it is in their best interest to do so. The simulation involves two agents (Agent A and Agent B) that decide whether to cooperate or defect based on their respective strategies. Agent B's decisions are guided by responses from OpenAI's language models via the OpenAI API, while Agent A can follow predefined strategies such as Tit for Tat, Generous Tit for Tat, Grim Trigger, etc.

Key components of the code include:
- Initialization of necessary Python packages and the LangChain wrapper for easier use of OpenAI's language models.
- Definition of an `Agent` class that encapsulates the attributes and methods related to an agent's actions, decision-making process, and score updating mechanism based on the game's outcomes.
- Implementation of several strategies (`tit_for_tat`, `tit_for_two_tats`, `generous_tit_for_tat`, etc.) that define how Agent A reacts based on the history of actions in the game.
- A function `simulate_prisoners_dilemma` that runs the game for a specified number of iterations, utilizing the strategies defined for Agent A and dynamically generated decisions for Agent B based on OpenAI's language model prompts.
- Visualization of the game's outcomes through score plotting over iterations for both agents.
- Logging of actions, decisions, and strategy effectiveness to files for analysis.

The simulation cycle involves:
1. Both agents making decisions based on their current strategy or the outcome of a language model prompt.
2. Updating their scores according to the rules of the Prisoner's Dilemma.
3. Logging each round's results and decisions for further analysis.

After running simulations with all predefined strategies, the code generates a summary of each strategy's performance, plots the scores of both agents over the iterations, and attempts to describe Agent B's strategy based on the game history using OpenAI's GPT model. It aims to explore the effectiveness of different strategies in a controlled, simulated environment and leverages the capabilities of advanced language models for decision-making and strategy analysis.
