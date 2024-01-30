# deep-learning-challenge
The purpose of this analysis is to predict the "successful" charities (i.e. the ones who met their fundraising goal) through using neural networks and tensor flow.

Results: (Optimization changes in bold)
|--------------------|Baseline       |Optimization #1     |Optimization #2    |Optimization #3                  |
|--------------------|---------------|--------------------|-------------------|---------------------------------|
|Accuracy:           |   72.81%      |    72.26%     |   72.28%      |   72.19%      |
|Target Variable(s): |IS_SUCCESSFUL  |IS_SUCCESSFUL  |IS_SUCCESSFUL  |IS_SUCCESSFUL  |
|Feature Variable(s):|<ul><li>ASK_AMT</li> <li>APPLICATION_TYPE(9 groups)</li> <li>CLASSIFICATION(6 groups)</li> <li>INCOME_AMT(8 groups)</li> <li>SPECIAL_CONSIDERATIONS:(2 groups)</li></ul>|<ul><li>ASK_AMT</li> **<li>APPLICATION_TYPE(6 groups)</li> <li>CLASSIFICATION(4 groups)</li>** <li>INCOME_AMT(8 groups)</li> <li>SPECIAL_CONSIDERATIONS:(2 groups)</li></ul>|<ul><li>ASK_AMT</li> **<li>APPLICATION_TYPE(6 groups)</li> <li>CLASSIFICATION(4 groups)</li>** <li>INCOME_AMT(8 groups)</li> <li>SPECIAL_CONSIDERATIONS:(2 groups)</li></ul>|<ul><li>ASK_AMT</li> **<li>APPLICATION_TYPE(6 groups)</li> <li>CLASSIFICATION(4 groups)</li>** <li>INCOME_AMT(8 groups)</li> <li>SPECIAL_CONSIDERATIONS:(2 groups)</li></ul>| 
|Variables Removed:  | <ul><li>EIN</li> <li>NAMES</li></ul>|<ul><li>EIN</li> <li>NAMES</li>**<li>USE_CASE</li>**</ul>|<ul><li>EIN</li> <li>NAMES</li>**<li>USE_CASE</li>**</ul>|<ul><li>EIN</li> <li>NAMES</li>**<li>USE_CASE</li>**</ul>|
|Layers, Neurons, Activation Functions:|<ul><li>Hidden Layer 1: 80, relu</li> <li>Hidden Layer 2: 30, relu</li> <li>Output Layer: 1, Sigmoid</li> </ul>|<ul><li>Hidden Layer 1: 80, relu</li> <li>Hidden Layer 2: 30, relu</li> <li>Output Layer: 1, Sigmoid</li> </ul>|<ul><li>Hidden Layer 1: **100**, relu</li> <li>Hidden Layer 2: **50**, relu</li> **<li>Hidden Layer 3: 20, relu </li>**<li>Output Layer: 1, Sigmoid</li> </ul>|<ul><li>Hidden Layer 1: **100**, **Sigmoid**</li> <li>Hidden Layer 2: **50**, **Sigmoid**</li> **<li>Hidden Layer 3: 20, **Sigmoid** </li>**<li>Output Layer: 1, Sigmoid</li> </ul>|
|Target Model Achieved?| no | no | no | no | 

I was not able to increase model performance in any of the 3 optimatizations- the basis model remains the most accurate model. 

In future models it might be worthy to look at AFFILATION and USE_CASE as those factors might influence the outcome more dramatically because Corporate Sponsorship and the purpose of the charity might have greater influence on the outcomes.
