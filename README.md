RL MARIO AGENT
------------

This project aims to build a robust RL agent that can make it through the first level of Super Mario Bros. Q-Learning poses an idea of assessing the quality of an action that is taken to move to a state rather than determining the possible value of the state (value footprint) being moved to. I've employed 3 methods of updating Q-values (ie training Mario), namely:
 * Vanilla Q-learning
 * Double Q-learning
 * Double Deep Q-learning (DDQN)

REQUIREMENTS
------------

The notebooks require the following modules:
 * [pytorch]: for building neural network in DDQN
 * [gym]: OpenAI toolkit to build reinforcement models
 * [gym-super-mario-bros]: OpenAI's environment for supermariobros
 * [nes-py]: emulator to run the environment
 * [random]: generating random rumbers
 * [pickle]: saving and loading files
 * [numpy]: efficient computation
 * [collections]: standard python library to use complex data structures
 * [cv2]: OpenCV for image processing
 * [matplotlib]: showing plots and images
 * [pylab]: extension to matplotlib, used for object oriented plotting

EXECUTION
------------

 * Open any notebook in colab or jupyter.
 * In the 'Cell' dropdown menu, select 'Run all below' option to run the notebook.
 * Solutions will appear after execution.

RESULTS
------------

 * Vanilla Q-learning and Double Q-learning are computationally expensive and hence slow. Only trained for around 200 and 120 episodes (till colab disconnects runtime) respectively but the results show a general trend of increasing rewards.
 * DDQN trained for 3000 episodes on Google Colab GPU. Results clearly show that the agent learns to maximize rewards with experience.
 * Also tried running the codes on personal machine with Intel i5-8250U but the machine froze before even running 1 episode.
 
FUTURE PROSPECTS
---------------

 * DDQN can be applied to more Atari games.
 * Explore more RL techniques and apply in Mario.
 * Train Mario evenly across various levels to build a stable, generalized agent.
 * I forgot to save the network weights after training the DDQN (T_T), should do that next time in order to see Mario play after training.
 
