# Notes — MDPs and RL for BESS

## Markov Decision Process (MDP)
Defined by \((S, A, P, R, \gamma)\):

- **States (S):** System conditions (e.g., SOC in 0.1 MWh steps → 10 states).  
- **Actions (A):** Charge, discharge, or stay idle.  
- **Transition (P):** Probability of moving between states.  
- **Reward (R):** Profit or cost from an action.  
- **Discount (γ):** Factor weighting future vs. immediate rewards.

Goal: Find a policy \(\pi(s)\) that maximizes expected cumulative reward.



## DADS and CACS
- **DADS (Dynamic Adaptive Decision System):** RL with explicit modeling of feedback between state, environment, and decisions. It adapts dynamically as new data arrives.
- **CACS (Context-Aware Control System):** Extends DADS by integrating contextual data (e.g., weather, prices, load) into decision making to improve adaptability.

Both describe data-driven control systems using RL or dynamic programming for continuous adaptation.



## Policies
- **Tabular policy:** Lookup table mapping states to actions (works for small discrete state/action spaces).  
- **Parameterized policy:** Uses continuous parameters (e.g., via NN) for complex or continuous systems.  
- **Deterministic vs. Stochastic:** Either fixed action per state, or probability distribution over actions.  



## When Neural Networks Are Needed
Use NN-based policies or value approximators when:
- State or action space is continuous.  
- Problem dimension is large (no compact table possible).  
- Environment dynamics are nonlinear and learned from data.

NNs appear in:
- **Policy networks (actors)** – output the action.  
- **Value/Q networks (critics)** – estimate expected reward.



## RL Approaches
- **Offline RL:** Train once from stored data.  
- **Online RL:** Continuously learn from interaction.  

Core methods rely on:
- Value and Q functions (\(V_\pi(s)\), \(Q_\pi(s,a)\))  
- Bellman equations linking rewards and future expectations  
- Balancing *exploration* (try new actions) vs. *exploitation* (apply best-known actions)
