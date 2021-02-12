# Human-Activity-Recognition-Task
Human activity recognition task done using wearable sensor data and different deep learning techniques. 
The data I have used is a famous data set in the internet known as 'mHealth dataset". A python script is developed to build two deep learning models using a convolutional neural network and an LSTM neural network. When sensor data is recorded into a csv file and then fed into the neural network model, it gives us what the person has done during the session. Here the algorithm is trained to identify four different activities standing, walking, jogging, and running.

Data from two IMU sensors are taken during four different activities. One IMU sensor is mounted on the chest and the other one is mounted on the left anckle. Tri axial accelerations from the chest mounted sensor, tri axial accelerations from the sensor mounted on the anckle, and tri axial angular velocities from the sensor mounted on the anckle are taken at a rate of 50Hz.

# For-CNN-algorithm
As CNNs are mostly suitable for operations such as image classification, data are reformatted as images before to train the CNN model. Data taken during each activity were broken into slices of 1 second. So, a single slice of 1 second consisted with 50 rows and 9 columns as we have taken 9 readings at a sampling rate of 50Hz.

# For-LSTM-algorithm
For train the LSTM algorithm, we used previously formatted dataset which prepared for use with the CNN algorithm. Here also we used one data sample per a second. So in each sample, there were 50 time-steps and 9 features.
