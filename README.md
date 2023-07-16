# Reinforcement_Learning
Project for the UniTS reinforcement learning course AA 2022-23.

# Flappy Bird solver
The idea is teach an agent how to play the flappy bird game using the text gym environment which can be found at: https://gitlab-research.centralesupelec.fr/stergios.christodoulidis/text-flappy-bird-gym/-/tree/master.

The agent will have no knowledge of the environment but perfect observability of the states. As such it is phrased as a model-free reinforcement learning problem. 

Standard RL techniques for policy control will be attempted and compared:
- Q-Learning
- SARSA
- Expected SARSA
- MC control

**COSE DA FARE**
- Decaying learning rate/ epsilon. Tuning su $\gamma, t^*$
- MC Control on policy.
- (?) TD $\lambda$

**Potenziali domande**
- Finite horizon.

Abbiamo aumentato solo alpha0 e epsilon0 su SARSA.
- Su epsilon via via che aumentavamo epsilon0 cresceva sempre, c'è da vedere se continua a crescere o a una certa peggiora (abbiamo fatto 0.05, 0.1, 0.15).
- Su alpha0 abbiamo visto che migliora e poi peggiora.
- Mettendoli insieme abbiamo preso l'alpha0 migliore di prima e epsilon0 0.15, sembra fare peggio che con alpha costante (punto 1). Quindi forse ha senso ottimizzarli insieme.


**Michele's problem(s):** \
[questo](Class-FV-MC-Control.ipynb) implementa una classe (codice è simile a quello che usa samu per Q-learning e SARSA), e si dovrebbe poter adattare... c'è appunto da definire il num_states che io non riesco a gestire usando un ambiente diverso. \
[questo](FV-MC-control.ipynb) non usa classi... è più basico ma l'ho preso da uno che lo usava per blackjack, e lì quindi gli stati sono discreti... eventualmente c'e da cambiare la definizione di Q (io ho provato a traformare in tuple ma non basta). Però io proverei prima con la classe e se funziona quella (come dovrebbe), [questo](FV-MC-control.ipynb) non lo guardiamo neanche.
