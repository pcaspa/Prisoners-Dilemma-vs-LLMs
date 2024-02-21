# Prisoners Dilemma vs Large Language Models  (Work in Progress)

![pd](https://github.com/pcaspa/Prisoners-Dilemma-vs-LLMs/assets/5567572/c4c1861b-62f7-485e-b34e-6e2e8fc34df7)


This project pits various large language models against 10 classic strategies in the Prisoner's Dilemma game.  Prisoner's Dilemma is an example of game theory that illustrates why two completely rational individuals might not cooperate, even if it appears that it is in their best interest to do so. The simulation involves two agents (Agent A and Agent B) that decide whether to cooperate or defect based on their respective strategies. Agent B's decisions are guided by responses from large language models, while Agent A can follow predefined strategies such as Tit for Tat, Generous Tit for Tat, Grim Trigger, etc.

Key components of the code include:
- Initialization of necessary Python packages and the LangChain wrapper for easier use of large language models.
- Definition of an `Agent` class that encapsulates the attributes and methods related to an agent's actions, decision-making process, and score updating mechanism based on the game's outcomes.
- Implementation of several strategies (`tit_for_tat`, `tit_for_two_tats`, `generous_tit_for_tat`, etc.) that define how Agent A reacts based on the history of actions in the game.
- A function `simulate_prisoners_dilemma` that runs the game for a specified number of iterations, utilizing the strategies defined for Agent A and dynamically generated decisions for Agent B based on large language model prompts.
- Visualization of the game's outcomes through score plotting over iterations for both agents.
- Logging of actions, decisions, and strategy effectiveness to files for analysis.

After running simulations with all predefined strategies, the code generates a summary of each strategy's performance, plots the scores of both agents over the iterations, and attempts to describe Agent B's strategy based on the game history using the large lanuage model. It aims to explore how effective large language models are against different classic strategies in a controlled, simulated environment.
