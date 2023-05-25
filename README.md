   # ![carton](https://github.com/somia76/IOT-Smart-Locking-System/assets/96308502/6666c93a-cad1-4132-bb49-a1b8e096afd6)

 A face recognition smart locking system is an advanced security solution that utilizes technology to grant access to individuals based on their facial features. This system employs a combination of hardware and software components to accurately identify and authenticate individuals in real-time.
 
 This project aims to improve the experience of security in homes, locks, etc. In addition to helping the elderly and handicapped with giving them an advanced feature.

We have used **ESP32-CAM module** as a main hardware component in our project. **ESP32-CAM** is a very small camera module with the ESP32-S chip and support WIFI. The AI-Thinker ESP32-CAM module comes with an ESP32-S chip, a very small size camera and a micro-SD card slot. Micro SD card slot can be used to store images taken from the camera or to store files.This ESP32-CAM module can be widely used in various IoT applications like face detection system. ESP32-CAM module also has several GPIO pins to connect the external hardware.


## Hardware Component:
* ESP32-CAM board.
* 12V Electronic Lock (SOLENOID LOCK).
* Relay Module.
* 12V DC suppl.
 
## Software Component:
* Arduino IDE. 
* Telegram.




## Our project consists of two parts
### PART 1, Door lock using face Regognition
we used video streaming web page to detect the faces. After uploading the face recognition door lock code to esp32-CAM. you will get an IP adress in serial monitor, copy this IP to your browser and you will get a video streaming web page: 

![ESP32-CAM-Testing](https://github.com/somia76/IOT-Smart-Locking-System/assets/96308502/e1c9844b-36b5-41cd-9d8d-dfd6fec7eb4f)

 To recognize the faces with ESP32-CAM, first, we have to enroll the faces. For that, turn on the Face recognition and detection features from settings and then click on the Enroll Face button. It takes several attempts to save the face. After saving the face, it detects the face as subject 0 where zero is the face number.
 After enrolling the faces, if a face is recognized in the video feed, ESP32 will make the relay module high to unlock the door.
 
###  PART 2, door lock with ESP 32 CAM & telegram:
Another important feature in our project is to make Wi-Fi door lock with photo capture using ESP32-CAM and Telegram app. you can take multiple photos, unlock and lock the door from anywhere in the world with the Telegram app.When anyone presses the doorbell, you will get a notification in the telegram app with a photo of that person. After that, you can easily unlock and lock the door from the telegram app.

We have used the UniversalTelegramBot library. So first you have to download and install it to create Telegram BOT to lock and unlock the door and capture a photo for the person who pressed the bell. 
![image](https://github.com/somia76/IOT-Smart-Locking-System/assets/96308502/91330bc8-e544-412e-a59d-85c96a038c89)

To create a telegram bot, We need to search on telegram for BotFather to start creating the smart lock bot, we ask to create new bot, give it a name and a unique username. At the end it give us the link of the bot we created and a token that will be used in our code.

![image](https://github.com/somia76/IOT-Smart-Locking-System/assets/96308502/a90ad0cd-589c-482a-b424-3f3341b9f0a7)

As shown we get our bot ID to use it in the telegram code with the token to link between them after installing the UniversalTelegramBot library.  

![image](https://github.com/somia76/IOT-Smart-Locking-System/assets/96308502/bb40e62f-20fb-45fd-a72e-4fb5bb51fdf2)



**Hardware video**: https://drive.google.com/file/d/1qLV34ttB2i-5RQax1TFvQFY6iPMhYyEj/view?usp=share_link



