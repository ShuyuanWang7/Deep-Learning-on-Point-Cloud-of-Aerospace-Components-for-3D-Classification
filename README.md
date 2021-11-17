# Deep-Learning-on-Point-Cloud-of-Aerospace-Components-for-3D-Classification
This is a deep learning project aiming to classify 3D models and match them with corresponding processes.

The following work is carried out in Prof. Wang Gang's Lab, Department of Mechanical Engineering, Tsinghua University (THU), Beijing.

# Engineering Background
Space launch vehicles widely use large aluminum alloy parts as structural supports, and their heat treatment processes have long relied on technicians to design and optimize them through trial and error methods, so the cost is high and the cycle is long. The process digitization of such core parts is one of the key research contents in the current aerospace manufacturing. We hope to combine the process knowledge of large-scale components accumulated for many years with machine learning, and to complete the approximate matching with existing components through independent identification of the geometric characteristics of new components, and to achieve process optimization on the basis of existing processes, which will greatly reduce the number of personnel. Design workload, provide process design efficiency and reliability.

# Prepare Dataset
The continuously updating 3D model dataset is in ./data file, involving 3 categories and 80 individuals respectively. My teammates transfer them into point cloud format, divided by training and testing dataset (./pointData file).

# Project Idea
We use two approaches to achieve the classification task, the multi-view and the point cloud. The multi-view method is based on projections from multiple perspectives, and the substantive idea is using 2D image convolutional neural network to analyse 3D models. We will update this method later. However, I want to exploit the original 3D models rather than any substitutions, saving uncessary computation costs and solving data sparsity. Inspired by PointNet (https://arxiv.org/abs/1612.00593), I can utilize point cloud models and corresponding 1D convolution to fix up the challenge.

# Environments
Pytorch (1.9.1)

CUDAtoolkit (10.2.89)

numpy (1.20.3)

tqdm (4.62.2)

time

os
