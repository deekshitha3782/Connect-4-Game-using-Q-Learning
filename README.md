Connect 4 game using Reinforcement Learning



I have used Q Learning Reinforcement Algorithm in this Project. You can download this git repository to see the accuracy of the trained model.
A colab version is also available.



Theory and Process:
1. What is Reinforcement Learning?
Reinforcement Learning is a type of machine learning that allows machines to learn how to take actions in an environment so as to maximize a reward.
In simple words, we can say that the output depends on the state of the current input and the next input depends on the output of the previous input
Example:
A dog gets his reward(treat munchkin) only if he obeys the order(state/work) of his master. So, the dog learns this from previous experience/state
of either a reward or a punishment(not getting treat munchkin).



2. Types of reinforcement learning used in Connect 4 Game so far:
a. Q Learning -  Q-learning is a model-free, off policy(greedy approach) reinforcement learning that will find the best course of action
from the Q table generated, given the current state of the agent.

Q-Table is a name for a simple lookup table where we calculate the maximum expected future rewards for action at each state.
It utilizes a table Q where rows represent the potential states, and columns represent actions
   
b. SARSA - Extension of Q Learning on policy(reward of the present state) model that will find the best course of actionfrom the Q table
   generated, given the current state of the agent.
   
c. Monte Carlo Method - Monte Carlo method is a very simple concept where agent learn about the states and reward when it interacts with the environment.

d. Deep Q Learning - Extenstion of Q Learning but selects the best course of action using deep neural network from the Q table generated.



3. Finialized to do continue with Q Learning because:

a. Model-free Approach: Connect 4 is a game with a large state space, and Q-Learning, being a model-free reinforcement learning algorithm,
doesn't require prior knowledge of the game's dynamics. It learns by exploring the state-action space, making it adaptable to different
strategies and tactics used in Connect 4.

b. Temporal Difference Learning: Q-Learning uses a temporal difference approach to update its Q-values. This means it can learn from single 
experiences, which is beneficial in games where you can't simulate all possible scenarios due to the vast number of moves.

c. Exploration vs. Exploitation: Connect 4 can have multiple optimal moves in different situations. Q-Learning balances exploration 
(trying new moves) and exploitation (choosing the best-known moves) effectively, allowing it to discover diverse strategies and adapt to the opponent's moves.



4. Applied Q Learning in the Connect 4 game
'http://romain.raveaux.free.fr/document/ReinforcementLearningbyQLearningThestickgame.html'
Used the above link to implement Q Learning on Connect 4 game. The above link uses Q Learning for Stick game.

Accuracy obtained after 5 games:
63.7%

Accuracy obtained after 10000 moves:
70.35%

Finally, the winning chances of the trained model obtained is 70% when played with a random player.
