[![GitHub ID](https://img.shields.io/badge/GitHub-MJAHMADEE-blue?style=flat&logo=github)](https://github.com/MJAHMADEE)

## 📂 Content (Videos, Slides, Codes)

Explore additional resources such as videos, slides, and code snippets available in our Google Drive folder. Click the badge below to access these materials:

[![Google Drive](https://img.shields.io/badge/Google_Drive-Folder-blue?style=flat-square&logo=google-drive)](https://drive.google.com/drive/folders/1rT-Cy_AaEl6DV2u7GwPAh8mlj0psw0Hd?usp=sharing)

# McCulloch-Pitts Neuron and Deterministic Finite Automaton (DFA)

This code implements a simple deterministic finite automaton (DFA) using McCulloch-Pitts neurons.

## Description

The code consists of two main parts:

### McCulloch-Pitts Neuron

The `McCulloch_Pitts_neuron` class defines a single McCulloch-Pitts neuron. It takes in weights and a threshold during initialization and implements a simple model to compute the output based on the input and weights.

### Deterministic Finite Automaton (DFA)

The `DFA` function creates a DFA using three McCulloch-Pitts neurons and simulates its behavior. The DFA is designed to have three outputs representing its state transition and acceptance based on the input and current state.

## Usage

To use the code:

1. Import necessary libraries (`numpy` and `itertools`).
2. Define the `McCulloch_Pitts_neuron` class with specific weights and a threshold.
3. Use the `DFA` function to simulate the DFA behavior with different inputs and states.

The provided code demonstrates the DFA behavior for a specific state and input, printing the current state, input, next state, and acceptance.

## Example usage:

```python
# Run DFA for specific inputs and states
# Create DFA instance
neur1 = McCulloch_Pitts_neuron([2, 2, -1], 2)
neur2 = McCulloch_Pitts_neuron([2, 0, 2], 2)
neur3 = McCulloch_Pitts_neuron([2, 1, -1], 2)

# Define initial states and inputs
state_b = [1, 0]
state = list(itertools.product(state_b, state_b))
input = [1, 0]
X = list(itertools.product(state, input))

# Execute DFA transitions
for i in X:
    res = DFA(i[0], i[1])
    print("DFA with current state as", str(i[0][0]) + str(" ") + str(i[0][1]), "with input as",
          str(i[1]), "goes to next state ", str(res[0]) + str(" ") + str(res[1]), " with acceptance ", str(res[2]))
```


# Neural Network Models and Data Analysis

This repository contains Python code demonstrating various aspects of neural network models, data preprocessing, and analysis using `scikit-learn`, `imbalanced-learn`, and `tensorflow.keras`.

## Description

The repository is structured as follows:

### Neural Network Models

#### MLP Classifier and Regression

The repository showcases the usage of `MLPClassifier` and `MLPRegressor` from `sklearn.neural_network`. The classifiers are trained on various datasets such as `load_diabetes` and `load_digits`. Evaluation metrics such as accuracy scores, confusion matrices, and classification reports are used to assess model performance.

#### Keras Sequential Models

Demonstrates the creation of various neural network architectures using `tensorflow.keras.Sequential`. Different configurations of hidden layers and activation functions are explored and analyzed using `Sequential` models.

### Data Preprocessing and Analysis

The repository includes data preprocessing techniques such as:

- Scaling data using `StandardScaler` from `sklearn.preprocessing`.
- Handling missing values and cleaning data using pandas.
- Feature engineering to extract company names from a car dataset.
- Replacing misspelled or incorrect company names for consistency.
- Calculating correlations between features and visualizing them using heatmaps.
- Creating scatter plots to visualize relationships between specific features and the target variable (`price`).

### File Structure

- `neural_networks.ipynb`: Jupyter notebook containing neural network model implementations and evaluations.
- `data_preprocessing.ipynb`: Notebook focusing on data preprocessing and analysis.
- `confusion_matrix.png`: Saved confusion matrix heatmap.
- `requirements.txt`: Python packages and versions required to run the code.

## Additional Learning Materials

Expand your understanding of machine learning concepts with tutorials on topics such as Cross-validation, Bootstrapping, and more. Access these resources in our Google Drive folder:

[![Google Drive](https://img.shields.io/badge/Google_Drive-Folder-blue?style=flat-square&logo=google-drive)](https://drive.google.com/drive/folders/1hJ6XWR-ozV390YkbOWx2fCWpQ51AZNr8?usp=sharing)

📣 Stay updated and engage in discussions by joining our Telegram channel:

[![Telegram Channel](https://img.shields.io/badge/Telegram_Channel-Join-blue?style=flat-square&logo=telegram)](https://t.me/+5palM1_8MvtjMDVk)

