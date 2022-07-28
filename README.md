<div id="top"></div>
<div align="center">
  <a href="https://github.com/BSH2409/R-B_Tree">
    <img src="https://user-images.githubusercontent.com/79904688/181488041-23f6174a-4ca0-4c2c-b6a3-553229dd8e73.jpg" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Door and Bell Automation Using Blynk</h3>

  <p align="center">
    <br />
    <a href="https://github.com/BSH2409/Door-And-Bell-Automation"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/BSH2409/Door-And-Bell-Automation">View Demo</a>
    ·
    <a href="https://github.com/BSH2409/Door-And-Bell-Automation/issues">Report Bug</a>
    ·
    <a href="https://github.com/BSH2409/Door-And-Bell-Automation/issues">Request Feature</a>
  </p>
</div>

## Problem Statement

<div align="center" id="about-the-project">
 </div>
As sometimes we forget our keys at home or it’s too much handful to carry keys while traveling, our project enables the user to operate the electric/ normal door through a third-party application (Blynk).
Another application could be if some guest or any known might come without any notice and we are not at home, rather than rushing to home to open the gate one can simply use the Blynk app to open the gate.
The Project also provides an option to ring the house bell in the case of alerting someone inside the house from a far distance or just for general purposes.
Apart from this if one want to collect the record of the time when the door was unlocked. Hence, we implemented our prototype with a feature to upload the current time to a MySQL database when unlocked.


### Requirements
* 4-channel relay module
*	NodeMCU
*	Arduino IDE
*	Jumper cables
*	Passive Buzzer
*	2 LED (red and blue)
*	Power Supply
*	Blynk Application
*	Mobile phone with internet connectivity


### Test Bed
* Arduino IDE
<p align="right">(<a href="#top">↑</a>)</p>


## Getting Started
This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites
In order to compile the following project ,the basic requirement is an Arduino IDE and the hardware components mentioned above.
For smooth installation of NODEMCU board refer to the given [link](https://www.youtube.com/watch?v=OC9wYhv6juM)

Voilà, All Set.

<p align="right">(<a href="#top">↑</a>)</p>
<div align="center">
  
## Block Diagram of the Project
  
![image](https://user-images.githubusercontent.com/79904688/181489201-5213e20e-888d-463c-a40b-1a3c14c5f349.png)

## Circuit Diagram
![image](https://user-images.githubusercontent.com/79904688/181489286-fe9eb719-0611-43cd-bdc7-fc8a0e1c81d1.png)

## IRL Prototype Snapshot
![image](https://user-images.githubusercontent.com/79904688/181489412-3ea6b6fc-1e8d-4db5-8300-cd9559a82d94.png)
  
</div>
## Working of the Prototype
We are using only two channels (channel 1 and channel 2) for our project.
Channel 1 is used for operating our electric buzzer as shown in the below image and the relay is connected in parallel so that it doesn’t interfere with the original working of the buzzer switch.
<div align="center">
  
 ![image](https://user-images.githubusercontent.com/79904688/181489562-af1647f8-f209-4454-8cc8-dfe9730d89d0.png)
  
</div>
Channel 2 is used for operating our electric door lock it has been connected to the door receiver via wires and then soldered to maintain a good connection as shown in the image.
  <div align="center">
  
 ![image](https://user-images.githubusercontent.com/79904688/181489576-a0f3abeb-8bca-4ff4-8087-eb54a34112be.png)
  
</div>
We have also added  Blue and Green LEDs in the circuit. green led glows when the lock is opened and the blue one glows when the circuit is connected with WIFI.  

## Node MCU and Blynk Connectivity
To connect our NodeMCU with Blynk Server, we have to create a project in Blynk mobile application and gather the authentication token. Then use Arduino IDE to create a sketch and upload it into the NodeMCU. The code of the project is provided in the appendix.

## Challenges on Implementation
1.	When we power up our setup, by default the relay module stays closed and had to be reset to prevent false ringing of the buzzer and false opening of the gate, as this might result in an automatic door opening when we have a power cut and then power comes back.
<div align="center">
  
![image](https://user-images.githubusercontent.com/79904688/181489826-8cd7033f-a66e-447e-88dc-040c8fd666bd.png)
  
</div>
Solution- The data pins connected to the relay channel input IN1 and IN2 must be reset to HIGH to prevent a closed circuit on the power back.
2.	To prevent rusting and damage from moisture to our modules, the following is fixed into a box that prevents accidental removal of jumper wire as well as provides a rigid structure to our setup


## Result

<div align="center">

  ### Off State
![image](https://user-images.githubusercontent.com/79904688/181489991-b8ee4762-0f93-4fac-914c-69246491c0bb.png)
  ### On State
  ![image](https://user-images.githubusercontent.com/79904688/181490024-3127e688-7c86-44a3-836c-4dc39a56b55a.png)
  ### MySQL DataBase
  ![image](https://user-images.githubusercontent.com/79904688/181490098-43b01c84-a3d5-4b47-8cc4-5248621ddfd0.png)

</div>
<p align="right">(<a href="#top">↑</a>)</p>

## Contact

Bhartik Harchand - [Instagram](https://www.instagram.com/_._bsh_._/) - bsh.bhartik@gmail.com

Project Link: [https://github.com/BSH2409/Door-And-Bell-Automation](https://github.com/BSH2409/Door-And-Bell-Automation)

