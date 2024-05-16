#prog 

[Useful Site](https://www.kaggle.com/datasets)

Machine Learning is a subfield of Artificial Intelligence ([[AI]]) that focuses on the development of [[algorithms]] and statistical models that allow computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of [[algorithms]] and mathematical models that enable systems to automatically learn from data, identify patterns, and make intelligent decisions or predictions.

## Key Concepts

### 1. [[Supervised Learning]]
[[Supervised learning]] is a type of machine learning where the algorithm learns from [[labeled data]]. It involves training a model on input-output pairs, where the input is the [[data]] and the output is the corresponding label or target value. The goal is for the model to learn a mapping function that can predict the output for new, unseen inputs.

Example:
```python
from sklearn.linear_model import LinearRegression

# Create a Linear Regression model
model = LinearRegression()

# Train the model using labeled data
X_train = [[1], [2], [3]]
y_train = [2, 4, 6]
model.fit(X_train, y_train)

# Predict output for new input
X_test = [[4]]
y_pred = model.predict(X_test)
print(y_pred)  # Output: [8]
```

### 2. [[Unsupervised Learning]]
[[Unsupervised learning]] is a type of machine learning where the algorithm learns from [[unlabeled data]]. It involves finding patterns or relationships in the [[data]] without any specific target variable. The goal is to discover hidden structures or groupings within the [[data]].

Example:
```python
from sklearn.cluster import KMeans

# Create a K-means [[clustering]] model
model = KMeans(n_clusters=3)

# Train the model using unlabeled data
X_train = [[1], [2], [10], [11]]
model.fit(X_train)

# Predict cluster labels for new input
X_test = [[3]]
y_pred = model.predict(X_test)
print(y_pred)  # Output: [0]
```

### 3. Reinforcement Learning
Reinforcement learning is a type of machine learning where an agent learns to make decisions in an environment to maximize a reward signal. It involves training an agent through trial and error, where it receives feedback in the form of rewards or penalties based on its actions. The goal is for the agent to learn the optimal policy or strategy to maximize long-term rewards.

Example:
```python
import gym

# Create an environment
env = gym.make('CartPole-v1')

# Define the agent's policy and learning algorithm

for episode in range(100):
    state = env.reset()
    done = False
    
    while not done:
        action = agent.select_action(state)
        next_state, reward, done, _ = env.step(action)
        agent.update(state, action, reward, next_state)
        state = next_state
        
env.close()
```

## Key Keywords

- **[[Regression]]**: A [[supervised learning]] task that predicts continuous numerical values.
- **[[Classification]]**: A [[supervised learning]] task that predicts discrete [[class]] labels.
- **[[Clustering]]**: An [[unsupervised learning]] task that groups similar [[data]] points together.
- **[[Feature Extraction]]**: The process of selecting or transforming raw data into meaningful features for machine learning [[algorithms]].
- **[[Overfitting]]**: When a machine learning model performs well on training [[data]] but fails to generalize well on unseen [[data]].
- **[[Underfitting]]**: When a machine learning model is too simple and fails to capture the underlying patterns in the [[data]].
- **[[Bias-Variance Tradeoff]]**: The tradeoff between a model's ability to fit training [[data]] (low bias) and its ability to generalize to unseen [[data]] (low variance).
- **[[Hyperparameters]]**: Parameters that are set before training a machine learning model and affect its [[performance]] but are not learned from the [[data]] itself (e.g., learning rate, number of hidden layers).
- **[[Feature Scaling]]**: The process of normalizing or standardizing features to a common scale to improve the [[performance]] of machine learning [[algorithms]].
- **[[Cross-validation]]**: A technique used to evaluate the [[performance]] of machine learning models by splitting the [[data]] into multiple subsets for training and testing.

Machine Learning in [[Python]] can be implemented using various libraries such as scikit-learn, TensorFlow, and PyTorch. These libraries provide a wide range of [[algorithms]] and tools for building and training machine learning models.