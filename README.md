# 2.1_The_companion_robot

# Word about 2.1

There are  lots of companion robots out there with impressive features and latest technologies. As  my first ESP32 project I decided to create an DIY companion robot for myself, Because it is realy fun to have one of them with us when we are working alone. This is the prototype of my *2.1*. We can improve in many ways. 

I created this with very simple and minimal resources that everyone can easily find with very low cost. All the components are available in famouse e-commerce websites for very low prices. Therefor I thins It is very easy to make your own *2.1* without much effort.

# Required Components

# ESP32 Board
![WhatsApp Image 2025-07-07 at 12 19 59 AM](https://github.com/user-attachments/assets/704bee46-c229-4599-90ab-d776ff340b61)

This is the main component that handle all processing tasks and act as the brain of our 2.1.
I prefer ESP32 over Arduino uno because this has builtin WIFI, bloototh capabilities and higher memory with higher processing capability.

# SSD1306 I2C  128 x 64 OLED display
![WhatsApp Image 2025-07-07 at 12 19 59 AM(1)](https://github.com/user-attachments/assets/92073dfe-1da3-47cd-829e-9582abc56354)

I choose this SSD1306 I2C  128 x 64 OLED display to show our 2.1's eye animations and it's feelings. This display is 128x64 pixel display and it is not a colour display it is a wihte colour only ( some sources says that white colour display is much durable than the blue one- do your own research and confirm by yourself).

#  MPU6050, a 6-axis motion tracking sensor
![WhatsApp Image 2025-07-07 at 12 20 00 AM(1)](https://github.com/user-attachments/assets/a10dc941-3985-49e2-a1b7-763fa0ec5886)

I am using this sensor module to detect 2.1's movements and change it's expressions accordingly. This sensor module includes gyroscope and accelerometer. So it can detect movements and make 2.1 more interactive.

# Capasitive touch sensor 
![WhatsApp Image 2025-07-07 at 12 20 00 AM](https://github.com/user-attachments/assets/cba33374-6b3a-41de-b196-ac086b0cd638)

I am using this touch sensor for directly interact with 2.1. We can give different commands by touches with this sensor. It detects touches and we can communicate with our robot easily with it.

# How to setup

Now we have to interconnect all the components we collected and make the final setup for our prototype of 2.1. It is very easy to do with a bread board and some jumper wiers.

*setup diagram*
![image](https://github.com/user-attachments/assets/0e837429-9eb0-43e4-9da3-3fd69a3081f9)
Diagram drawn with wokwi online emulator (https://wokwi.com/projects/435758617419686913)

You should connect all the components as above diagram. with correct pins.

MPU6050 
SCL ==> 22  |
SDA ==> 21  |
VCC ==> 5V  |
GND ==> Any GND pin in ESP32    |

OLED Display
SCL ==> 22  |
SDA ==> 21  |
VCC ==> 5V  |
GND ==> Any GND pin in ESP32    |

Touch Sensor
SIG ==> GPIO 18 |
VCC ==> 3V  |
GND ==> Any GND pin in ESP32    |

