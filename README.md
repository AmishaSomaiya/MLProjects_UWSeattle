This repo contains ML projects and experience across industry and academia in the fields of 
Vision, NLP, 3DVision, ML for Robotics, Traditional ML, Deep Learning, MLOps, Contrastive Learning and Data Visualization. 

### 1. ML for JPL EELS robot perception and navigation(Ongoing)

Design and implementation of end-to-end perception pipeline for precise EELS robot navigation in perceptually challenging and extreme environments such as shadows, occlusions, low light, snow, fog and rain using raw data (LiDAR, Stereo and IMU). 


### 2. Question Answering on SQuAD using BiDAF and traditional ML(Ongoing)


### 3. UW - NASA/JPL Machine Learning for Extreme Traverse Lunar Explorer

This project deploys Machine Learning algorithms to enhance the onfield data characterization capabilities of the NASA-JPL EELS (Extant Exobiology Life Surveyor) robot,  performs semantic terrain segmentation on the vision dataset collected by EELS in ice crevasses and glacial-like extreme subterranean environments, combats limited data availability in space missions, works with real unannotated data from JPL and inferences on sensor-fusion requirements.


### 4. SimCLR+DCL, Self-Supervised Constrastive Representation Learning 

This project self-implements simCLR, a popular framework for self-supervised contrastive learning for generating representations. However, simCLR is computationally expensive and the 
original paper implementation uses a default batch size of 4092 and 32 TPUs for 
good performance. Another issue with simCLR is the positive-negative 
coupling effect in the InfoNCE loss, due to which the model performance 
degrades at sub-optimal hyperparameters like small batch sizes. This project 
addresses these issues by using Decoupled Contrastive Learning (DCL) loss 
instead of simCLR loss. The final project implementation of simCLR with DCL 
loss with Resnet50 backbone at 100 epochs achieves a top1 accuracy of 84.84% 
at batch size of 32 for linear evaluation on CIFAR10 dataset. This outperforms 
the top1 accuracy of 81.66% at the same batch size of 32 with simCLR loss and 
has comparable performance to previously obtained top1 accuracy of 85.08% at 
higher batch size of 128. Thus, the final project implementation of simCLR with 
DCL efficiently generates vision representations at lower batch sizes with 
computational savings and good performance metrics that can be used for 
several downstream vision tasks.


### 5. Machine Learning for 5G Wireless Systems Beam Selection using XGBoost

5G and MIMO(Multiple Input Multiple Output) utilize radio frequencies in the sub-6 GHz range and the millimeter-wave (mmWave) frequency range (30-300GHz). These smaller wavelengths (in millimeters) allow to design tinier antennas and, in turn, pack many more at both transmitter and receiver ends. Thus, there are multiple antenna array elements at both the transmitter and receiver ends. Selecting the best beam pair out of these becomes essential for maximum information gain. To unleash the full power of mmWave communications, a prominent challenge consists in reducing the overhead introduced by the beam selection (or alignment) procedures. This project proposes a machine learning algorithm to reduce this overhead using XGBoost with SMOTE. The data used is from the Raymobtime datasets s008 and s009 with GPS, LiDAR, and image input features. The proposed algorithm outputs a prediction of top k(k=10) best beam pairs for every receiver input, thus providing the communication system with a complementary, out-of-band information to reduce the processing overhead. The final model combats overfitting with early stopping and uses random search cross-validation for hyperparameter tuning. The proposed algorithm has a top 10 accuracy of 94.2%, beating the SOA by 3.2% and has a computational cost of 0.25 hours, which is 3x lesser than SoA. Also, the proposed algorithm reaches accuracy of 98% early at k=20 instead of at k=30 for SoA. The top 20 accuracy with SMOTE to reduce minority class misclassifications is reasonable at 96.5%.


### 6. ML integration to Heroku using Dockers, Flask  and GitHub Actions

This repository builds a Machine Learning model from scratch and deploys the ML model in 4 ways as follows:
automated POST API using flask and Postman
front-end web application on local server using flask and html
deploy to Heroku cloud without Dockers
deploy to Heroku cloud with Dockers, CI/CD pipeline and Github Actions

https://github.com/AmishaSomaiya/MLOps_1


### 7. Tuning Playsite, Hyperparameter tuning multi-page interactive website

Deep Learning Model Hyperparameters are configuration settings that are external to the machine learning model itself
and need to be manually set before the training process begins. Setting/tuning these
hyperparameters is extremely difficult for several reasons. There are many hyperparameters, and
each hyperparameter can take on multiple values. One hyperparameter can affect another, thus
understanding the complex dependencies requires a lot of experimentation which many can’t
afford as tuning them is time-consuming and expensive. Worst of all there is no universal
solution, as one set of hyperparameters won’t work for a different problem/model. So we provide
a comprehensive approach to this problem with our interactive multi-page data viz website. 

https://github.com/cse512-23s/Tuning-PlaySite

