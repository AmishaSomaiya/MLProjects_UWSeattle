## Problem Statement : 

This project requires to deploy Machine
Learning algorithms to enhance the onfield data characterization capabilities of
the NASA-JPL EELS (Extant Exobiology
Life Surveyor) robot. This project requires performing
semantic terrain segmentation on the
vision (and potentially LiDAR data)
collected by EELS in ice crevasses and glacial-like extreme subterranean environments. The project also requires to
combat limited data availability in space missions, work with real unannotated
data from JPL and inference on sensor-fusion requirements.

## Approach and Results :

•	Designed and implemented zero-shot sim-to-Real end-to-end UDA pipeline, robust to unknown and unseen terrains. 

•	Achieved 88.9 mIoU for Unsupervised Domain Adaptation with 
synthetically generated data (training date) as source domain and unannotated NASA-JPL
data as target domain (test data). 

•	Combatted limited data availability by design and implementation of semantically labeled data generation pipeline 
using Procedural Generation and Domain Randomization in UnReal Engine. 

•	Created reusable data generation pipeline using blueprint scripts that can be reused by JPL for any projects that have scarce vision data. 


## Code : 

under NDA 


