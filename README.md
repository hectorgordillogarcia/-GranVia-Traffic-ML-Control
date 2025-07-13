
# 🚦 GranVia-Traffic-ML-Control

This repository contains a Machine Learning-based traffic control system developed to manage traffic lights on Madrid’s **Gran Vía** using **SUMO (Simulation of Urban MObility)**.

We designed and trained intelligent agents capable of dynamically adjusting traffic light cycles based on real-time traffic conditions. The objective is to reduce congestion, waiting times, and improve overall traffic flow by employing reinforcement learning algorithms.

## 🧠 Algorithms Implemented

The following reinforcement learning techniques were tested and compared in this project:

- **DQN** (Deep Q-Network)
- **PPO** (Proximal Policy Optimization)
- **QL** (Q-Learning)
- **SARSA**
- **RESCO**
- **SB3** (Stable Baselines3 - framework used for various implementations)

Each of these methods was applied to the SUMO simulation, and their performance was analyzed based on key traffic metrics (e.g., waiting time, queue length, travel time).

## 🗺️ Scenario

The simulation recreates a simplified version of **Gran Vía**, one of Madrid’s main avenues, including its intersections and traffic patterns.

- **SUMO** was used to model the road network, define vehicle flows, and simulate traffic behavior.
- **Python** and **TraCI** were used to interact with SUMO and control the traffic lights using ML agents.


## ▶️ How to Run

1. **Install SUMO and dependencies**  
   Ensure that SUMO and its Python tools (`TraCI`) are correctly installed on your system.


2. **Train or evaluate an agent**  
   Example:
   ```bash
   python main.py --agent dqn --train
   python main.py --agent ppo --evaluate
   ```

3. **Visualize simulation**  
   The SUMO-GUI can be enabled to visualize vehicle movements and traffic light behavior in real time.

## 📊 Results

Each algorithm was tested under the same traffic conditions. The following performance metrics were evaluated:

- Average waiting time
- Average travel time
- Queue lengths
- Emissions

Visualizations and comparison graphs are available in the `results/` folder.

---

## 👨‍🔬 Authors

**Héctor Gordillo** · **David Laborda** · **Javier Fernández** · **Martín Loring**

## 📄 License

This project is licensed under the MIT License.
