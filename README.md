# deep-learning-challenge
Overview of the analysis: The purposed of this analysis is to predict the "successful" charities (i.e. the ones who met their fundraising goal) through using neural networks and tensor flow.

Results:                                                                                                 
**Baseline:** 
Accuracy: 72.8%
Target Variable(s): IS_SUCCESSFUL
Feature Variable(s): 
  ASK_AMT
  APPLICATION_TYPE: organized into 9 groups
  CLASSIFICATION: organized into 6 groups
  INCOME_AMT: organized into 8 groups
  SPECIAL_CONSIDERATIONS: organized into 2 groups
Variables removed: None 
Neurons & Layers Selected: 
  Hidden Layer 1: 80
  Hidden Layer 2: 30
  Output Layer: 1
Activation Functions Selected: Sigmoid

Target Model Performance Achieved?  No
  
**Optimization #1:** 
Steps to Optimize model in bold  
Accuracy: 72.26%
Target Variable(s): IS_SUCCESSFUL
Feature Variable(s): 
  ASK_AMT
**  APPLICATION_TYPE: organized into 6 groups**
**  CLASSIFICATION: organized into 4 groups**
  INCOME_AMT: organized into 8 groups
  SPECIAL_CONSIDERATIONS: organized into 2 groups
**Variables removed: USE_CASE**
Neurons & Layers Selected: 
  Hidden Layer 1: 80
  Hidden Layer 2: 30
  Output Layer: 1
Activation Functions Selected: Sigmoid

Target Model Performance Achieved?  No

****Optimization #2: ****
Steps to Optimize model in bold 
Accuracy: 72.28%
Target Variable(s): IS_SUCCESSFUL
Feature Variable(s): 
  ASK_AMT
  **APPLICATION_TYPE: organized into 6 groups**
  **CLASSIFICATION: organized into 4 groups**
  INCOME_AMT: organized into 8 groups
  SPECIAL_CONSIDERATIONS: organized into 2 groups
**Variables removed: USE_CASE**
Neurons & Layers Selected: 
  Hidden Layer 1: 100
  Hidden Layer 2: 50
  Hidden Layer 3: 20
  Output Layer: 1
Activation Functions Selected: Sigmoid

Target Model Performance Achieved?  No

**Optimization #3: **
Accuracy: 72.19%
Target Variable(s): IS_SUCCESSFUL
Feature Variable(s): 
  ASK_AMT
  **APPLICATION_TYPE: organized into 6 groups**
  **CLASSIFICATION: organized into 4 groups**
  INCOME_AMT: organized into 8 groups
  SPECIAL_CONSIDERATIONS: organized into 2 groups
**Variables removed: USE_CASE**
Neurons & Layers Selected: 
  Hidden Layer 1: 100
  Hidden Layer 2: 50
  Hidden Layer 3: 20
  Output Layer: 1
Activation Functions Selected: Sigmoid


What variable(s) are the target(s) for your model?
What variable(s) are the features for your model?
What variable(s) should be removed from the input data because they are neither targets nor features?
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
