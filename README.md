# 🚕 Q-Learning : Taxi-v3 avec Python

![Thumbnail](thumbnail.png)

🚕 Ce dépôt contient l'implémentation d'un agent d'apprentissage par renforcement (Reinforcement Learning) capable de résoudre le problème du "Taxi" de l'environnement OpenAI Gym.

## 📌 Project Overview
The goal of this project is to train a reinforcement learning agent to navigate a 5x5 grid world. The agent must:
1. Pick up a passenger at a designated location.
2. Drop them off at the correct destination.
3. Minimize the number of steps and avoid illegal actions.

The agent learns the optimal strategy through the **Q-Learning** algorithm, exploring the environment and receiving rewards based on its performance.

## 🧠 Key Concepts
This implementation focuses on the fundamental parameters of Reinforcement Learning:
- **Alpha ($\alpha$)**: The Learning Rate.
- **Gamma ($\gamma$)**: The Discount Factor (importance of future rewards).
- **Epsilon ($\epsilon$)**: The exploration rate using an Epsilon-greedy strategy with decay.
- **Q-Table**: A matrix of 500 states $\times$ 6 actions updated via the Bellman equation.

## 🛠️ Installation & Setup
This project was developed using a virtual environment and **Jupyter Notebook**.

### 1. Clone the repository and create a Virtual Environment
```bash
# Create the environment
python -m venv venv

# Activate it (Windows)
.\venv\Scripts\activate

# Activate it (macOS/Linux)
source venv/bin/activate
```

### 2. Install Dependencies
Using the provided `requirements.txt` file:
```bash
pip install -r requirements.txt
```

## 🚀 How to Run
1. Ensure your virtual environment is activated.
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open the main notebook file and run the cells sequentially to train and visualize the agent's performance.

## 📂 Project Structure
- `*.ipynb`: The Jupyter Notebook containing the code and step-by-step logic.
- `requirements.txt`: List of Python packages required for the project.
- `venv/`: Python virtual environment (ignored in git but used for local development).
- `thumbnail.png`: Visual representation of the project.
- `README.md`: Project documentation.

## 📊 Results
The trained agent is capable of finding the shortest path to the passenger and destination without any wrong moves, demonstrating the efficiency of Q-Learning in discrete state spaces.