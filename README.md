# HAR
FYP Fall 2018:
HUMAN ACTIVITY RECOGNITION
Track-O-Matic

A webapp that gives a detailed summary of all of your current and past bad habits. 

***

# DESCRIPTION

The project consists of detecting activities that are done unconsciously when a person is anxious. The aim of this project is to simulate a smartwatch which will identify these activities and send a signal to the individual to stop them from doing it. Our web app will be based on body-focused repetitive behaviors (BFRBs) such as nail biting, foot tapping, smoking etc. 

We used two smarts phones for this purpose. The sensors of the smartphone such as accelerometer, gyroscope and magnetometer. We will be using a neural network to identify these activities. There were two major parts of this project. The first part consisted of training the model and the second was to test the model and its accuracy.

***

# User Manual

1. Install PhonePi App through Play Store. 
    PhonePi allows you to stream real-time data from sensors on your phone. The sensors that we used were accelerometer, gyroscope and      magnetometer.
    
2. The URL in the app needs to be entered in the format:    
        ip_address_of_Raspi:5000
       
    Enter update time for the required sensors that is the duration after which the data must be re-read and hit the switch. To disable,  simply turn the switch off.
    
3. To get the IP use ipconfig command on cmd. Make sure the phone and PC are on the same network.

4. Install Python 3 from Python's official website prefably on Windows 7 on which this project was implemented. 

5. Download our code and run it!

***

# INSPIRATION

This idea was inspired by the Samsung Health app which records numerous activities for a person using the smartphones various sensors. However, the Samsung Health App fails to identify activities on its own. It does activity recognition of walking, but activities like how many glasses of water a user drank and the food activities need to be recorded manually. It also guesses that a person is sleeping if the phone is not being used at night but that too asks for confirmation in the morning if they were actually asleep.

***

# Hardware / Software details

The hardware used in this project are sensors of Samsung S8+ and Samsung S5. The sensors used were accelerometer, gyroscope, magnetometer. Accelerometers are devices that measure acceleration, which is the rate of change of the velocity of an object. They measure in meters per second squared (m/s2) or in G-forces (g). Magnetometers are devices that measure magnetic fields. A magnetometer is an instrument with a sensor that measures magnetic flux density B (in units of Tesla or as/ m2). Magnetometers refer to sensors used for sensing magnetic fields OR to systems which measure magnetic field using one or more sensors. Gyroscopes, or gyros, are devices that measure or maintain rotational motion. MEMS (microelectromechanical system) gyros are small, inexpensive sensors that measure angular velocity. The units of angular velocity are measured in degrees per second (°/s) or revolutions per second (RPS). Angular velocity is simply a measurement of speed of rotation.

Some sensors were bought from Spark Fun which were Spark Fun 9DOF Razor IMU MO, Lithium Ion Battery-400mAH, 10 DOF Mems IMU Sensor, Qwiic IMU - MPU-9250. We planned to use them fully however we could not do so because these sensors did not contain Bluetooth or Wi-fi so the activities could not be detected in run time. The activities had to be performed and then the sensors had to be plugged in and then the data had to be extracted and then the Machine Learning Algorithm had to be used.

The project is Python based and Jupyter Notebook has been used. The libraries used were Pandas and Keras. Deep Neural Network (DNN) gave the highest accuracy which was 93%. Dense layers were used, which were total 5 (increasing it decreased the accuracy), 1 input layer with input dimension 549 (number of columns of the training data). The activation function was SoftMax. The next 3 layers were hidden and used the activation function Rectified Linear Unit (relu) each of which had 600 units. The output layer dimension was 6 and activation function was sigmoid (data was changed to categorical initially).

While fitting the model batch size 200 was used (increasing it increased the accuracy) and epochs used were 6 (increasing it increased the accuracy).

***

# CREDITS

We would like to thank our supervisor Ms. Nida Saddaf Khan for the patient guidance, encouragement and advice she has provide. Without her help and constant guidance, we would not have been able to complete our project. Who identified the problems in our project and gave us the solutions to those problems as well and helped us in all our queries very promptly. 

***

# PROJECT VIDEO

[Click here for the project video](https://www.dailymotion.com/video/x6ytrx9)
