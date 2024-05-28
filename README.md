# Overview
This project delves into the sophisticated application of reinforcement learning (RL) leveraging the Advantage Actor-Critic (A2C) algorithm across multiple Gymnasium environments. Specifically, the implementation of A2C is demonstrated on two well-established environments, CartPole and BipedalWalker, in addition to the development of a custom environment designed to rigorously evaluate the algorithm’s effectiveness and flexibility.

## A2C
The Advantage Actor-Critic (A2C) algorithm is a reinforcement learning technique that combines aspects of both policy-based and value-based methods. It utilizes an actor-critic framework, where the actor selects actions based on the current policy, while the critic evaluates these actions by estimating the value function. A key innovation of A2C is the introduction of the advantage function, which measures the relative value of an action compared to the average actions in a given state. By incorporating this function into the policy update process, A2C reduces variance in gradient estimates, leading to more stable learning. Moreover, A2C often employs parallel environments for training, allowing for faster and more efficient learning.

## Environments

### CartPole
The CartPole environment is a seminal control problem within the RL community. The objective is to maintain the balance of a pole on a moving cart by exerting appropriate left or right forces. This environment serves as an excellent testbed for examining an agent's capability to develop stable control strategies through continuous real-time feedback and adjustment. The simplicity of the CartPole environment allows for rapid iteration and debugging, providing a clear visualization of the learning process and algorithmic performance.

### BipedalWalker
The BipedalWalker environment introduces a significantly more intricate challenge. The agent must learn to ambulate using two legs across a rugged and dynamically changing terrain. This environment necessitates the acquisition of coordinated, multi-joint movements and balance, making it an ideal scenario for testing advanced RL algorithms such as A2C. The complexity of BipedalWalker lies in its requirement for precise motor control and the ability to adapt to unforeseen obstacles and perturbations in the environment, thus providing a comprehensive assessment of the A2C algorithm's robustness and efficacy.

### Custom Grid World Environment
In a 5x5 grid-based virtual environment inspired by "Courage the Cowardly Dog," the agent, embodying Courage, navigates to find an exit from a cave, symbolizing game completion. Four potential actions—moving up, down, left, or right—are available, facilitating comprehensive exploration. Encounters with obstacles like ghosts, zombies, and the grim reaper heighten complexity. To counterbalance challenges, strategic rewards such as torchlights, ghost-repelling pills, fire torches, and cloaks are placed within the grid, enhancing gameplay depth. The primary objective is to guide Courage to the exit, maximizing reward accumulation while efficiently navigating obstacles. This objective fosters adaptive learning through trial and error, with each action contributing to the agent's evolving strategy to optimize its path and balance risk with reward.

