# NFA-Based Multi-Agent Market Simulation

## Overview
This project explores the use of **Nondeterministic Finite Automata (NFA)** as a decision-making framework for autonomous agents operating in a simulated market economy. Developed as part of a **Theory of Computing course**, the project bridges formal automata theory with agent-based modeling to study emergent economic behavior.

Each agent follows an NFA-based strategy that governs transitions between behavioral states during repeated market interactions. The simulation demonstrates how **local nondeterministic decision rules** can produce complex global dynamics such as cooperation patterns, wealth inequality, and market stability.

---

## Conceptual Model
Agents operate using an NFA with the following components:

- **States**:  
  - Cooperate  
  - Defect  
  - Negotiate  
  - Withdraw  

- **Input Alphabet**:  
  - High payoff  
  - Low payoff  

- **Transition Function**:  
  - Either deterministic or nondeterministic  
  - Nondeterministic transitions assign probabilities to multiple possible next states  
  - Probabilities are adjusted using agent-specific risk tolerance parameters  

This formalism allows agents to exhibit adaptive and probabilistic behavior while remaining grounded in classical automata theory.

---

## Simulation Design
The simulation is implemented using the **Mesa agent-based modeling framework**. Each agent starts with an initial resource allocation and repeatedly engages in pairwise negotiations with randomly selected partners.

A payoff matrix determines resource transfers based on the interaction of agent states. After each transaction, agents transition to new states according to either deterministic or nondeterministic automaton rules. Over time, this produces emergent patterns at the population level.

Two primary simulation modes are evaluated:
- **Deterministic agents**, using fixed transition rules
- **Nondeterministic agents**, using probabilistic NFA transitions

---

## Data Collection and Metrics
During each simulation run, the following metrics are recorded:
- Average agent resources
- Gini coefficient (resource inequality)
- Proportion of agents in each behavioral state
- Cooperation and defection rates over time

These metrics enable direct comparison between deterministic and nondeterministic agent populations.

---

## Visualization and Analysis
The project includes extensive visual analysis:
- Time-series plots comparing deterministic and nondeterministic systems
- State distribution dynamics across simulation steps
- Spatial simulations using a grid-based layout
- Animated visualizations showing real-time agent interactions and emergent behavior

Animations and figures illustrate how nondeterminism affects cooperation stability, inequality growth, and overall market efficiency.

---

## Results
The results show that nondeterministic agents exhibit:
- Higher behavioral diversity
- Increased resource volatility
- Different cooperation and inequality trajectories compared to deterministic agents

These findings highlight how nondeterminism—central to theoretical computer science—can meaningfully influence large-scale system behavior when applied to multi-agent economic models.

---

## Repository Structure

- NFA_Based_Multi_Agent_Market_Simulation.ipynb
- LICENSE
- README.md

---

## Contributors
This project was completed as a **group project**.

- **Asmaa Ibrahim**
- **Belal Ehab**
- **Hana Taher**
- **Ibrahim Shalaby**
- **Kenzy Ahmed**
- **Khadija Wesam**
- **Lama Nezar**
- **Yassin Ashraf**
- **Zeinab Mohamed**
- **Zena Alaa**

---

## License
This project is licensed under the **MIT License**.  
See the `LICENSE` file for more details.
