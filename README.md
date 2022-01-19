# Weak-Supervision-Framework-with-Active-Learning
The project has been done solely for the purpose of research as a part of Course CSC 2508 - Advanced Data Systems.

Machine learning models require huge amounts of labeled data in order to achieve good performance on text classification tasks. However, good quality labels are often difficult to obtain, which limits the applicability of these techniques. Weak supervision is one such data labeling technique which uses weak supervision sources for assigning noisy labels to unlabeled instances. On the contrary, active learning is a method which makes use of user input to generate good quality labels for the data. We aim to investigate how a hybrid model of the two would perform, in addition to emphasizing on the performance advantage of stand-alone active learners when compared to weak supervision frameworks. We develop an active learning module to query the most difficult instances from the unlabeled dataset and find that logistic regression classifier with uncertainty sampling is the best performing estimator - query strategy combination for active learner. We compare the performance of this active learner with various other weak supervision baseline models and identify that it outperforms them by only labeling a maximum of 100 actively sampled instances.

## Dataset 
1. https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection </br>
2. https://cogcomp.seas.upenn.edu/Data/QA/QC/train_5500.label </br>


## Models Reproduced as a part of Analyis
#### 1.Snorkel </br>
Ratner, A.J., Bach, S.H., Ehrenberg, H.R., Fries, J.A., Wu, S., Ré, and C. Snorkel: Rapid training
data creation with weak supervision. In Proceedings of the VLDB Endowment International
Conference on Very Large Data Bases, 11 3, 269-282 ., 2017.</br>

#### 2.Imply_Loss</br>
Abhijeet Awasthi, Sabyasachi Ghosh, Rasna Goyal, and Sunita Sarawagi. Learning from rules
generalizing labeled exemplars, 2020.</br>

#### 3.Astra</br>
Giannis Karamanolakis, Subhabrata Mukherjee, Guoqing Zheng, and Ahmed Hassan Awadallah.
Self-training with weak supervision, 2021.</br>

#### 4.modAL: A modular active learning framework for Python3</br>
Tivadar Danka and Peter Horvath. modal: A modular active learning framework for python,
2018.</br>

## Findings 
#### Performance of different classifiers against number of instances labeled using three different sampling techniques in active learning for TREC dataset
<img width="684" alt="image" src="https://user-images.githubusercontent.com/37900145/150080060-6d98fbce-eeb0-4031-91c5-bc533ec60f90.png">


