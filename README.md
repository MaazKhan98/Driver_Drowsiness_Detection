## Driver Drowsiness Detection Using Facial Features  
#### Project Aim & motive:  
This project is a part of junior year curriculum. In this project we aim to real time detect driver's alertness level while driving, and sound an alarm if the   driver is not paying attention.  
Initially an open-sourced dataset of eye images is acquired and pre-processed by altering its size, alignment etc. accordingly. It is then followed by data augmentation, which is a strategy that significantly increase the diversity of data available for training models, without actually collecting new data. Next, a deep learning model is designed that would train upon processed dataset images and make predictions according to binary classes, i.e., OPEN and CLOSED. Proposed models achieves an accuracy of 93% with only 10 epochs of training and very limited data to train upon. Next part of the project deals with real-time deployment of model, which is done using Open-CV. Baseline algorithm for real-time detection starts with feeding the camera input to OCV and then using one of its classifiers “HaarCascade” to extract region of interest (ROI) from each frame and sending it to the model in back-end to make its prediction. Predictions are displayed back on the screen and appropriate actions, like sounding an alarm upon drowsiness detection is taken.

#### Change Logs:  
- **model_det v1.0** : Base model architecture.      
- **model_det v1.1** : Real-time detection, actions on detection added - Text display,window-border color.  
- **model_det v1.2** : Alarm sound, alarm starts beeping after certain time of not paying attention,detection is displayed better,fix: Alertness level now decreases on drowsiness.  

