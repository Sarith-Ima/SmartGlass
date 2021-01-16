# SmartGlass
Creating a GUI using FreeRTOS 

--Motivation--

One of the growing trends of wearable computing is Head Mounted Displays (HMD), as the head is a great gateway to receive audio, visual and hectic information. Also due to the Google Glass project, wearables in form of glasses gained much more attention during last year’s. Google Glass is as futuristic a gadget we’ve seen in recent times. A useful technique for all kinds of people including handicapped/disabled. 
There are many examples which have integrated Arduino in creation of such a system. But those systems are only available to accomplish specific task. For example refer to following example.

Smart Glass for Multimeter-In this system it simply receives data from a Multimeter via Bluetooth module, this system doesn’t provide any other facility to user. So users are limited to a certain space. Link-https://create.arduino.cc/projecthub/AlainsProjects/arduino-data-glasses-for-my-multimeter-   bb4e59

So in summary almost every existing system is constrained and limited to provide a specific facility. Simply read data via Bluetooth module and write data on an OLED display.
Many systems doesn’t support any processing on received data because of technical limitations since almost every system use much less powerful Arduino modules.

--Objectives--

-1.Retrieve data from any external Bluetooth module
   There is no limitation for users to select the preferred device to connect. User can connect any device which contains a Bluetooth module and communicate with the glass.
  
-2.Process retrieved data
   This system provides following facilities to user using retrieved data

   --User can view data read from external device

   --User gets a OS-like,GUI interface to interact with the system
     This GUI interface provides Buttons, Drop menus to interact with system. 

   --User gets joystick module to manipulate throughout the GUI
     Joystick is used to manipulate so user can click Button and scroll Drop menus.

   --User can set an alert/counter which gives him an alert if he exceeds the limit given by him
     This is very useful in a situation like user reads value from a Multimeter. Suppose    that user reads voltage from Multimeter and he should get notified when the voltage      value exceeds a certain value, in such cases user can set an alert on reading values.


-3.Projecting image of the OLED Display on lens of the glass
   In order to project image of the display we need to design a lens system considering all lens constraints. We have to consider about font size, font color in order to have      clear projection. Design of the lens system will be discussed in implementation section.



