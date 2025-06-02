# NEAT\_PONG

!\[player vs. AI]\(assets/ping\_pong.gif)

A Python implementation of the classic Pong game trained via [NEAT](https://github.com/CodeReclaimers/neat-python).
Original code from **[techwithtim](https://github.com/techwithtim)**
The neural network learns paddle control (up/down) purely through evolutionary algorithms.

## 🔍 Overview

This project trains a NEAT-based agent to play Pong against itself (or a fixed opponent). Starting from a minimal network, NEAT evolves both structure **and** weights until the agent learns to keep the ball in play and score. Key features:

* **Minimal-to-Complex**
  Begins with simple genomes and grows connections/nodes only when needed.
* **Fitness by Paddle Hits**
  Each time the AI’s paddle hits the ball, its fitness increases, encouraging longer volleys.
* **Configurable Topology**
  You can tweak mutation rates, population size, and activation functions in `config-feedforward.txt`.
