# A_Deep_Learning_Approach_for_Nonprofit_Funding_Selection

Overview

The aim of this project is to develop a deep learning model to assist Alphabet Soup, a nonprofit foundation, in selecting funding applicants with the highest likelihood of success in their ventures. By leveraging machine learning techniques, particularly neural networks, we seek to create a binary classifier capable of predicting whether organizations funded by Alphabet Soup will be successful.

Instructions

Step 1: Data preparation
* Read the charity_data.csv to a Pandas DataFrame.
* Identify target and feature variables
* Drop unnecessary columns (EIN and NAME).
* Determine unique values for each column.
* Bin rare categorical variables.
* Encode categorical variables.
* Split data into features and target arrays.
* Scale the datasets using StandardScaler.

Step 2: Compile, Train, and Evaluate the Model
* Design a neural network model using TensorFlow and Keras.
* Create hidden layers with appropriate activation functions.
* Check the structure of the model.
* Compile and train the model.
* Evaluate model performance using test data.
* Results saved as AlphabetSoupCharity.h5.

Step 3: Optimize the Model
* Adding back "NAME" column and group counts less then 100 into "other"
* With modification the model achieve >75% accuracy.
* Results saved as AlphabetSoupCharity_Optimization.h5.

Step 4: Neural Network Model Findings
* Provide an overview of the analysis.
* Discuss data preprocessing: target(s), feature(s), and unnecessary variables.
* Describe neural network architecture and optimization steps.
* Evaluate model performance and provide recommendations.

Conclusion

In this project, we have employed a Feedforward Neural Network model to tackle the task at hand. This model architecture, comprised of two hidden layers with ReLU activation functions and a sigmoid output layer, has shown promising results in predicting outcomes for the given problem.

The chosen architecture reflects a common approach in deep learning, leveraging the flexibility and complexity of neural networks to capture intricate patterns within the data. The ReLU activation function, utilized in the hidden layers, facilitates the model's ability to learn non-linear relationships, while the sigmoid activation function in the output layer is well-suited for binary classification tasks.

However, it's important to acknowledge that the model's effectiveness depends not only on its architecture but also on the nature of the problem and the characteristics of the dataset. Alternative models, such as decision tree-based methods like Random Forest or Gradient Boosting, could offer a different perspective.

For instance, decision tree-based models provide interpretability and handle categorical data effectively, which might be advantageous depending on the interpretability requirements of the task. Additionally, logistic regression, with its probabilistic interpretations of predictions and computational efficiency, could serve as a baseline model for comparison.

Each model comes with its own set of advantages and disadvantages, and a thorough comparative analysis could shed light on the most suitable approach for the specific problem at hand. Future iterations of this project could benefit from exploring a broader range of models and evaluating their performance against the Feedforward Neural Network implemented here.

Ultimately, the choice of model should align with the objectives of the project and the preferences of the stakeholders, ensuring that the selected approach effectively addresses the challenges posed by the data and yields actionable insights for decision-making.