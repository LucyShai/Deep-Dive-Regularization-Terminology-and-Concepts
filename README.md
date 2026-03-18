📋 Project Overview
This project explores regularization techniques to prevent overfitting in deep neural networks. Using a real-world scenario of predicting optimal kick positions for the French football team, we demonstrate how L2 regularization and Dropout can significantly improve model generalization.

🎯 Learning Objectives
Understand overfitting and its impact on model performance

Implement L2 regularization (weight decay) from scratch

Implement Dropout regularization from scratch

Compare the effects of different regularization techniques

Analyze the bias-variance tradeoff in neural networks

📊 Dataset: French Football Field Positions
Problem Statement
Predict where the French goalkeeper should kick the ball so that French players can hit it with their heads.

Dataset Description
Input: 2D positions on a football field

Output: Binary classification

🔵 Blue dots: French player hits the ball

🔴 Red dots: Opposing team hits the ball

Characteristics: Noisy dataset with a diagonal decision boundary


Key Terminology Explained 
Overfitting
Definition: Model learns training data too well, including noise

Symptoms: High train accuracy, low test accuracy

Analogy: Memorizing textbook vs learning concepts


L2 Regularization (Weight Decay)
Definition: Adds penalty for large weights to cost function

Effect: Forces weights to be small and distributed

Formula: J_reg = J_original + (λ/2m)Σ||W||²


Dropout
Definition: Randomly deactivates neurons during training

Effect: Creates ensemble of networks, prevents co-adaptation

Analogy: Team members learn to work with any combination of colleagues


Inverted Dropout
Definition: Scales activations during training to maintain expected value

Purpose: No scaling needed during testing

Formula: A_train = (A * mask) / keep_prob

Bias-Variance Tradeoff
Bias: Error from wrong assumptions (underfitting)

Variance: Error from sensitivity to data (overfitting)

Regularization: Increases bias slightly, decreases variance significantly
