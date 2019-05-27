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

# CREDITS

We would like to thank our supervisor Ms. Nida Sadaf Khan for the patient guidance, encouragement and advice she has provide. Without her help and constant guidance, we would not have been able to complete our project. Who identified the problems in our project and gave us the solutions to those problems as well and helped us in all our queries very promptly. 

***

# PROJECT VIDEO

[Click here for the project video](https://www.dailymotion.com/video/x6ytrx9)
