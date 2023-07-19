# Reinforcement Learning Project
This repository contains the project for the UniTS reinforcement learning course AA 2022-23.

[Here](...) you can find the final presentation slides.

# Flappy Bird solver
The goal is teach an agent how to play the flappy bird game using the text gym environment which can be found at: https://gitlab-research.centralesupelec.fr/stergios.christodoulidis/text-flappy-bird-gym/-/tree/master.

The agent will have no knowledge of the environment but perfect observability of the states. As such it is phrased as a model-free reinforcement learning problem. 

Standard Reinforcement Learning techniques for policy control will be attempted and compared:
- [MC control](/Ufficiale/MC_Control.ipynb)
- [SARSA](/Ufficiale/SARSA.ipynb)
- [Expected SARSA](/Ufficiale/E_SARSA.ipynb)
- [Q-Learning](/Ufficiale/Q.ipynb)

# Results

For each methods, various set of hyperparameters were tested.
In [Plots](/Ufficiale/Plots/) folder are stored the resulting plots for each parameters configuration:
-   [MC Control](/Ufficiale/Plots/MC_plots)
-   [SARSA](/Ufficiale/Plots/SARSA_plots)
-   [Expected SARSA](/Ufficiale/Plots/Exp_SARSA_plots)
-   [Q-LEarning](/Ufficiale/Plots/Q_plots)

In [Summary](/Ufficiale/Summary/) folder are stored some statistics for each parameters configuration, as following:
` $lambda$ | $k_{\alpha}$  | $k_{\varepsilon}$ | mean | median  |standard deviation `





**COSE DA FARE**
- Decaying learning rate/ epsilon. Tuning su $\gamma, t^*$
- MC Control on policy.
- (?) TD $\lambda$



Abbiamo aumentato solo alpha0 e epsilon0 su SARSA.
- Su epsilon via via che aumentavamo epsilon0 cresceva sempre, c'è da vedere se continua a crescere o a una certa peggiora (abbiamo fatto 0.05, 0.1, 0.15).
- Su alpha0 abbiamo visto che migliora e poi peggiora.
- Mettendoli insieme abbiamo preso l'alpha0 migliore di prima e epsilon0 0.15, sembra fare peggio che con alpha costante (punto 1). Quindi forse ha senso ottimizzarli insieme.


