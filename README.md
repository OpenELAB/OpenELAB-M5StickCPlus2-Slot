&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;__Hi👋__，Welcome to this tutorial on implementing a super cool Slot Machine🎰 project using M5StickC Plus2! This project series will be divided into three parts, and today you'll be in the first part, focusing on how to build the project, run the code, and implement the core functionality.Next, you will be taken through the following steps 📜 to dive into the source code and get started with this project with ease! Ready? Let's get started 🚀! 
- 📝 Project Description
- ✨ Functional Features
- 🏗 Project Structure
- 🚀 Installation and Operation
- 🔧 Instructions for use
- 🔮 Next Issue Preview
  
[Demo video 📺]()
# M5StickCPlus2_Slot Project
## Project Information.
This project creates a mini version of a slot machine 🎰 by using M5StickC Plus2. Players can start the reels and stop them column-by-column by simply pressing a button to enjoy an exciting gaming experience! The project features a 1.14-inch TFT display that showcases five cool columns of reels, each containing 10 different icons, and the reels spin with a lot of motion 🎡.
  By interacting with the M5StickC Plus2's buttons, players can easily control the start and stop of the game, as if they were in a real slot machine 🎮. This project not only demonstrates the power of M5StickC Plus2 in graphic display and hardware control, but also provides a fun and interactive experience for players, making it a great learning and reference project for hardware development and game development enthusiasts 💡!

## Functional Features
- 📏 Compact size: lightweight design, suitable for carrying around, easy to build.
- 🎉 Fun: highly interactive, as if you are in the real world of slot machine games.
- 🔋 Low power consumption: high efficiency and low power consumption, prolonging the use of the equipment
## Project structure
``` 
│── README.md             # Project description file
│── M5StickCPlus2_slot    # Source code folder
  │── M5StickCPlus2_slot.ino   # Source Code Files
  │── Slot.cpp                 # Slot Function Implementation File
  │── SLot.h                   # Slot function definition file
  │── image                    # Image folder
    │── slot_bar.h                 # esp32 icons
    │── slot_cherry.h              # Cherry icon
    │── slot_lemon.h               # lemon icon
    │── slot_openelab.h            # OpenELAB logo
    │── slot-orange.h              # Orange icon
    │── slot_seven.h               # Number 7 icon
    │── slot_symbols.h             # Icon Data
```
## Installation and operation

### precondition
Software dependency: __Arduino IDE__, __VScode__ or __text__, etc.  

Hardware requirements: __USB-C cable__, __M5StickCPlus2__, etc.  

Dependencies: __M5StickCPlus2 library__, __Arduino library__, etc.  

### Arduino IDE Installation Steps
```
Link: upload later
```
### Installation of dependencies
1、After installing the Arduino IDE, open the Arduino settings, copy the M5 development board link to the arrow shown and click OK to save it.
```
https://static-cdn.m5stack.com/resource/arduino/package_m5stack_index.json
```
![QQ_1726105473838](https://github.com/user-attachments/assets/367bd060-13ab-4eda-9a43-13fbc0250580)  
  
2、Open Tools->Board->Boards Manager

![QQ_1726105693629](https://github.com/user-attachments/assets/e70b4f19-c21a-4ea5-80e2-4d150b54a35f)  
  
3、Search for M5Stack and choose to install it, it's already installed on this host so I won't repeat the installation.

![QQ_1726105854495](https://github.com/user-attachments/assets/11b18b6c-c8db-4ea4-b209-d22dd26eebbe) 

4、Select development version, Tools->Board->M5Stack Arduino->M5StickCPlus2 

![QQ_1726106317846](https://github.com/user-attachments/assets/203d874b-f316-4ae7-827b-2e01493ce08d)


5、Next, install the M5StickCPlus2 library, select Tools->Manage Libraries, search for M5StickCPlus2, and then select Install, which will not be repeated if it is already installed.

![QQ_1726106703496](https://github.com/user-attachments/assets/312bc9e1-521c-479e-831a-a3c22e45a6ec)  

### compile and run
1、After completing the installation of the dependencies, open the good downloaded zip archive

![QQ_1728369077423](https://github.com/user-attachments/assets/c5a627bb-d95d-43a0-9e1e-1440b4646487)


2、Connect the Plus2 to your computer using USB-C, select Tools->Port to choose your own port

![QQ_1726107673971](https://github.com/user-attachments/assets/17f0392a-b753-4aba-946c-ede75ba9092f)  

3、Click on compile and then click on upload when the compilation is complete

![QQ_1726107957719](https://github.com/user-attachments/assets/c1f953ad-5355-44e8-af0c-ac5da7542aa6)  

## Instructions for use
- ### Order and number of pictures
The slot machine has five columns, each of which can hold up to 10 icons, and you can adjust their order at will!💡At the moment, we have prepared six 48x48 pixel material icons, their RGB565 hexadecimal data is already in the code, corresponding to elements 0 to 5 in the slot_symbols array. If you want to change the order and number of icons in each column, you can easily change the number in the symbolIndices array to change the display of the icons in each column!🔧🎨  

![QQ_1726108827608](https://github.com/user-attachments/assets/45b5878d-3624-47b5-a671-fc40937d1898)

- ### Column-to-column and figure-to-figure spacing
By changing PAD_X and PAD_Y, you can change the spacing between columns and graphs, usually the default is 2 and 0. 

![QQ_1726109192019](https://github.com/user-attachments/assets/3e14c412-8342-486d-ba00-b6a0f4d357ac)

- ### Turntable rotation speed, stop reduction speed
```
#define Speed_MAX 800           //Maximum speed of slot machine rotation
#define Speed_MIN 50            //Slot machine rotation minimum speed
#define Acceleration_MAX 12     //Acceleration when the slot machine is accelerating
#define Acceleration_MIN -20    //The acceleration when the slot machine is slowing down.
```
  ![QQ_1726109492610](https://github.com/user-attachments/assets/aaa6b4a0-79b1-491a-8dbd-ca76cc8c1eee)

## Next Issue Preview
In the next issue, we will explain in detail how to change the picture of the slot machine, we will get the hexadecimal parameters of the picture by taking the model of the picture and adjusting it to the format we want, and then present the picture we want on the slot machine __Stay tuned!!!__

![QQ_1726122393803](https://github.com/user-attachments/assets/71507de5-dad0-4688-84bf-56cc25878e35)  

[Next Issue Link](https://github.com/OpenELAB/OpenELAB-M5StickCPlus2-Slot-2.git)  

## How to contact the maintainer or developer
__OpenELAB:__   
[![OpenELAB_logo_resized_150](https://github.com/user-attachments/assets/5d3de375-359c-46a3-96bb-aaa211c6c636)](https://openelab.io)  
__YouTube:__  
[![youtube_logo_200x150](https://github.com/user-attachments/assets/d2365e7f-4ffe-4124-bf62-21eba19a71e4)](https://www.youtube.com/@OpenELAB)  
__X :__  
[![X_logo_150x150](https://github.com/user-attachments/assets/4ad5095f-2573-4791-9360-b355530093bf)](https://twitter.com/openelabio)  
__FaceBook:__  
[![facebook_logo_cropped_150x150](https://github.com/user-attachments/assets/52f2dc9a-a564-49a5-b72e-30eafbbc281f)](https://www.facebook.com/profile.php?id=61559154729457)  
__Discord__  
[![resized_image_150x150](https://github.com/user-attachments/assets/93ecd098-3391-45bb-9d80-b166c197a475)](https://discord.gg/VQspWyck)

