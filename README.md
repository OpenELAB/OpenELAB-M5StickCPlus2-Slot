&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;__Hi__ 👋, welcome to this tutorial on building a super cool slot machine 🎰 project with the M5StickC Plus2! This project is divided into three parts, and today we’ll focus on the first part: building the project, running the code, and implementing the core functionality. In the following steps 📜, you'll explore the source code and get started easily. Ready? Let's dive in 🚀!  
- 📝 Project Description
- ✨ Functional Features
- 🏗 Project Structure
- 🚀 Installation and Operation
- 🔧 Instructions for use
- 🔮 Next Issue Preview
  
[Demo video 📺]()
# M5StickCPlus2_Slot Project
## Project Description
This project creates a mini version of a slot machine 🎰 using the M5StickC Plus2. Players can start the reels and stop them column by column by simply pressing a button, enjoying an exciting gaming experience! The project features a 1.14-inch TFT display showcasing five columns of reels, each containing 10 different icons, with the reels spinning dynamically 🎡. By interacting with the M5StickC Plus2's buttons, players can easily control the start and stop of the game, simulating a real slot machine 🎮. This project not only demonstrates the power of the M5StickC Plus2 in graphic display and hardware control but also offers a fun, interactive experience—making it an excellent learning project for hardware and game development enthusiasts 💡!

## Functional Features
- 📏 Compact size: Lightweight design, easy to carry, and simple to assemble.
- 🎉 Fun: Highly interactive, making you feel as if you're immersed in the real world of slot machine games.
- 🔋 Low power consumption: High efficiency and low energy usage, extending the device's operating time.
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
1、After installing the Arduino IDE, open the settings, paste the M5 development board link into the designated field, and click OK to save the changes.
```
https://static-cdn.m5stack.com/resource/arduino/package_m5stack_index.json
```
![QQ_1726105473838](https://github.com/user-attachments/assets/367bd060-13ab-4eda-9a43-13fbc0250580)  
  
2、Open Tools->Board->Boards Manager

![QQ_1726105693629](https://github.com/user-attachments/assets/e70b4f19-c21a-4ea5-80e2-4d150b54a35f)  
  
3、Search for M5Stack in the Arduino Library Manager and install it. Since it's already installed on this system, I won’t repeat the installation process.

![QQ_1726105854495](https://github.com/user-attachments/assets/11b18b6c-c8db-4ea4-b209-d22dd26eebbe) 

4、Select development version, Tools->Board->M5Stack Arduino->M5StickCPlus2 

![QQ_1726106317846](https://github.com/user-attachments/assets/203d874b-f316-4ae7-827b-2e01493ce08d)


5、Next, install the M5StickCPlus2 library by selecting Tools -> Manage Libraries, searching for "M5StickCPlus2," and clicking Install. If the library is already installed, the installation process will be skipped.

![QQ_1726106703496](https://github.com/user-attachments/assets/312bc9e1-521c-479e-831a-a3c22e45a6ec)  

### compile and run
1、After completing the installation of the dependencies, open the downloaded ZIP archive.

![QQ_1728369077423](https://github.com/user-attachments/assets/c5a627bb-d95d-43a0-9e1e-1440b4646487)


2、Connect the Plus2 to your computer using a USB-C cable. Then, go to Tools -> Port and select the correct port.

![QQ_1726107673971](https://github.com/user-attachments/assets/17f0392a-b753-4aba-946c-ede75ba9092f)  

3、Click Compile, and once the compilation is complete, click Upload.

![QQ_1726107957719](https://github.com/user-attachments/assets/c1f953ad-5355-44e8-af0c-ac5da7542aa6)  

## Instructions for use
- ### Order and number of pictures
The slot machine has five columns, each capable of holding up to 10 icons, and you can freely adjust their order! 💡 Currently, six 48x48 pixel icons are prepared, with their RGB565 hexadecimal data embedded in the code, corresponding to elements 0 to 5 in the slot_symbols array. To modify the order or number of icons in each column, simply adjust the values in the symbolIndices array to customize the icon display in each column! 🔧🎨 

![QQ_1726108827608](https://github.com/user-attachments/assets/45b5878d-3624-47b5-a671-fc40937d1898)

- ### Column-to-column and figure-to-figure spacing
By adjusting PAD_X and PAD_Y, you can modify the spacing between columns and icons. The default values are usually set to 2 and 0, respectively.

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
In the next installment, we will provide a detailed guide on how to change the slot machine's images. We will generate the hexadecimal parameters of the images by modeling them and adjusting them to the desired format. Once done, the customized images will be displayed on the slot machine. __Stay tuned!!!__

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

## Material Purchase Links
[M5StickCPlus2](https://openelab.io/products/m5stickcplus2?_pos=2&_sid=d60b08054&_ss=r)  

[USB-C](https://openelab.io/products/usb-a-to-usb-type-c-cable-white?_pos=2&_psq=USB-C&_ss=e&_v=1.0)

