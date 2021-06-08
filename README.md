# neural_networks_for_hand_pose_recognition_based_on_armband_electrical_signals

Modeling finger pose based on time-series sensor measurements by using SVM and neural network models for the 5-dimensional regression problem

Introduction

The surface electromyography (sEMG)-based gesture recognition with a deep learning approach and real-time recognition can become important in practical, advanced human-computer interaction. The sEMG signal is obtained by an armband with non-invasive skin-contact sEMG electrodes. The electrical activity recorded allows development of a human-computer interface system which can be employed in a number of areas: Assistive or Rehabilitative technology (e.g., myoelectric controlled prosthesis or assistive robots or even sEMG-driven exoskeletons); Serious games and advanced, intuitive and more natural input and simulation control; and Silent speech recognition. For additional information and background, see, e.g.:

0. Wikipedia, Human?computer interaction. https://en.wikipedia.org/wiki/Human%E2%80%93computer_interaction

1. Reaz MB, Hussain M, Mohd-Yasin F. Techniques of EMG signal analysis: detection, processing, classification and applications. Biological Procedures Online. 2006;8(1):11?35. https://link.springer.com/article/10.1251/bpo124

2. Hakonen M, Piitulainen H, Visala A. Current state of digital signal processing in myoelectric interfaces and related applications. Biomed Signal Process Control. 2015;18:334?359. https://www.sciencedirect.com/science/article/pii/S174680941500021X

3. Hu Y, Wong Y, Wei W, Du Y, Kankanhalli M, Geng W. A novel attention-based hybrid CNN-RNN architecture for sEMG-based gesture recognition. PLOS ONE 2018;13:e0206049. https://doi.org/10.1371/journal.pone.0206049

Data overview

The data consists of synchronized sensor readings and labels from multiple sequences of different gestures and hand movements collected for one hand collected at approx. 50Hz. The sensor data/features consists of 30-dimensional vectors (the number of channels in our current wristband) and 5-dimensional groundtruth/labels vectors (the number of fingers in a hand). Thus, each sequence is composed of a feature vector X (t x 30) and a label vector Y (t x 5). The sensors readings are collected at 10-bit resolution, [0, 1024].

Goal of this project

Predict the pose of the hand (angles of the fingers) based on armband electrical sensor data using a machine-learning method such as SVR or a neural network approach.
