Polaroid SX-70 camera using Raspberry Pi Zero W
===============================================

Automatically upload photo single exposure, photo double exposure and video with polaroid style frame, date and time variables to twitter account at https://twitter.com/SX70_RPi

![alt text](https://github.com/udut7/Polaroid-SX70-RPi/blob/master/SX70_Raspberry_Pi.jpg?raw=true "Polaroid SX-70 camera Raspberry Pi Zero W, automatically upload photo to https://twitter.com/SX70_RPi")

Operating System:
- Raspbian Stretch Lite

Hardware:
- Polaroid SX-70
- Raspberry Pi Zero W
- Raspberry Pi Camera
- Capacitive Touch Key Module for main menu loop selection button (GPIO4) positioned behind light meter glass:
    1. Photo to twitter (red blink indicator)
    2. Video to twitter (green blink indicator)
    3. Double Exposure Photo to twitter (blue blink indicator)
    4. Restart or Shutdown (white blink indicator)
- Original SX-70 shutter release for action button of each main menu selected above (GPIO18):
    1. Action at Photo to twitter menu:
         - Take photo (red light for take photo continued with green light for upload to twitter)
    2. Action at Video to twitter menu:
         - Start Recording (red light start record)
         - Stop Recording (red light stop record continued with green light for upload to twitter)
    3. Action at Double Exposure Photo to twitter menu:
         - Take first main photo (red light for take photo)
         - Take second transparant photo (red light for take photo continued with green light for upload to twitter)
    4. Action at Restart or Shutdown menu (red light timer):  
         - Short pressed, between 2 until 5 seconds: restart
         - Long pressed, above 5 seconds: shutdown
- RGB LED for light indicator (GPIO16, GPIO20 & GPIO21) positioned at film counter
- Main power switch positioned at light control
- Power Module Lithium Battery

Optional hardware:
- 0.96 inch (80x160) TFT display 65K full color SPI (GPIO3, GPIO10, GPIO11, GPIO22 & GPIO27) positioned at view finder
- DC Stepper Motor Drive Controller (GPIO13, GPIO17, GPIO19 & GPIO26) for polaroid mechanical shutter sound effect
- Yashica Pro-50DX external flash light with PCB mounted white LED
- 433MHz RF wireless transmitter receiver module (GPIO12) for triggering external flash light wirelessly
- 5 volt relay module (GPIO23) for controlling external flash light
- Buzzer module (GPIO24) for sound indicator

Next development: black and white photo, shutter sound effect, external flash light, wireless shutter release
