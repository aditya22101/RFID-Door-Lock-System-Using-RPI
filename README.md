# RFID-Door-Lock-System-Using-RPI
Just similar to an Arduino, ESP32, ESP8266, and STM32, Raspberry Pi Pico is also a controller board based on the RP2040 microcontroller, through the programming of which, you can control almost anything. And apart from this, you can also monitor different types of analog and digital sensors as well.
The RFID door lock system project aims to develop an advanced access control mechanism using RFID technology. To utilize RFID tags and readers, the system provides enhanced security, convenience, and efficient access control. The system features real-time access monitoring, customizable access privileges, and remote administration. It eliminates the need for physical keys, reduces the risk of unauthorized access, and enables seamless and contactless entry. The project provides some unauthentic action by beeping buzzer, The RFID door lock system offers improved safety. 
IMPLEMENTATION 
Firstly, identify these components. Secondly, connect the GPIO Extension board to the breadboard. And then, connect the GPIO ribbon cable to the extension board. Thirdly, connect the RFID module to the GPIO extension board. For that, use the circuit diagram below. Next, place the buzzer on the breadboard. And then, connect it to the extension board. 
Also, connect the LCD and relay module to the extension board. Please use the circuit diagram above. Now, connect the keyboard, mouse, monitor, ethernet cable, and SD card(OS installed) to the Raspberry Pi board. Then, connect the GPIO ribbon cable to the Raspberry Pi board and provide a power supply to the board. Ok, now let’s install the RFID library into Raspberry Pi OS. 
Follow the instructions below for that. First, open the terminal and run the following commands one by one. At this point, the Raspberry Pi board must be connected to the Internet.
1. sudo apt install python3-dev python3-pip 
2. sudo pip3 install spidev 
3. sudo pip3 install mfrc522 
OK, the RFID library is ready for this project. Now, enable I2C and SPI communication. Because the LCD screen and RFID module required these communication methods. If you want to know whether I2C is working or not, run the following code on the terminal. Then, we can see the I2C address. i2cdetect -y 1; Now let’s create the python script for this project.
Follow the below steps for that. First, let’s get the RFID tag ID. For that, copy and paste the following program on the Thonny IDE. Then, save this script and click the run button. No need to install I2C library. It is included in the file above. But keep these scripts in one folder. Now, place the RFID tag on the RFID reader. Then, we can see the tag ID on the LCD screen and shell. And then, copy and paste this ID to the main python script. Finally, the RFID Door Lock System is ready.
Contact
For any inquiries or support, please contact:

Email: aditya22101@iiitnr.edu.in

Feel free to modify this README according to the specifics of your project and your needs.
