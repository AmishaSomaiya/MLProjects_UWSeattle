# MLProjects_UWSeattle
Vision, NLP, 3DVision, ML for Robotics, Traditional ML, Deep Learning, MLOps, Contrastive Learning and Data Visualization

### 1. ML for JPL EELS robot perception and navigation(Ongoing)

Design and implementation of end-to-end perception pipeline for precise EELS  navigation in perceptually challenging and extreme environments such as shadows, occlusions, low light, snow, fog and rain using raw data (LiDAR, Stereo and IMU). 

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

