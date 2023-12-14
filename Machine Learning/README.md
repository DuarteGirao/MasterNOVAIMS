# MastersNovaIMS-Machine_Learning


## 1. Introduction <br>
- A new disease has recently been discovered by Dr. Smith, in England. You have
been brought in to investigate. The disease has already affected more than 5000
people, with no apparent connection between them.
- The most common symptoms include fever and tiredness, but some infected people are asymptomatic. Regardless, this virus is being associated with post-disease
conditions such as loss of speech, confusion, chest pain and shortness of breath.
- The conditions of the transmission of the disease are still unknown and there are no
certainties of what leads a patient to suffer or not from it. Nonetheless, some groups
of people seem more prone to be infected by the parasite than others.
<br>

## 2. Objective of the project <br>
- In this challenge, your goal is to build a predictive model that answers the question,
“Who are the people more likely to suffer from the Smith Parasite?”. With that
goal, you can access a small quantity of sociodemographic, health, and behavioral
information obtained from the patients.
- As data scientists, your team is asked to analyze and transform the data available as
needed and apply different models to answer the defined question in a more accurate
way. Can you build a model that can predict if a patient will suffer, or not, from the
Smith Disease?
- The score of your predictions is the percentage of instances you correctly predict,
using the f1 score.<br>
<br>

## 3. Datasets <br>
You have access to two different datasets:
1. The training set should be used to build your machine learning models. In this
set, you also have the ground truth associated to each patient, i.e., if the patient
has the disease (Disease = 1) or not (Disease = 0). Is composed by:
- **train demo.csv** - the training set for demographic data and the target
- **train health.csv** - the training set for health related data
- **train habits.csv** - the training set for habits related data
2. The test set should be used to see how well your model performs on unseen
data. In this set you don’t have access to the ground truth, and the goal of
your team is to predict that value (0 or 1) by using the model you created using
the training set. Is composed by:
- **test demo.csv** - the test set for demographic data
- **test health.csv** - the test set for health related data
- **test habits.csv** - the test set for habits related data
