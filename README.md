<div align="center">

  <img src="https://user-images.githubusercontent.com/62047147/195847997-97553030-3b79-4643-9f2c-1f04bba6b989.png" alt="logo" width="100" height="auto" />
  <h1>XIAO ROBOT</h1>
  
  <p>
    VOICE RECOGNITION ROBOT with XIAO nRF52840 Sense
  </p>
  
  
<!-- Badges -->

<a href="https://github.com/cifertech/XIAO-ROBOT" title="Go to GitHub repo"><img src="https://img.shields.io/static/v1?label=cifertech&message=XIAO-ROBOT&color=white&logo=github" alt="cifertech - XIAO-ROBOT"></a>
<a href="https://github.com/cifertech/XIAO-ROBOT"><img src="https://img.shields.io/github/stars/cifertech/XIAO-ROBOT?style=social" alt="stars - XIAO-ROBOT"></a>
<a href="https://github.com/cifertech/XIAO-ROBOT"><img src="https://img.shields.io/github/forks/cifertech/XIAO-ROBOT?style=social" alt="forks - XIAO-ROBOT"></a>
   
<h4>
    <a href="https://twitter.com/cifertech1">TWITTER</a>
  <span> · </span>
    <a href="https://www.instagram.com/cifertech/">INSTAGRAM</a>
  <span> · </span>
    <a href="https://www.youtube.com/c/cifertech">YOUTUBE</a>
  <span> · </span>
    <a href="https://cifertech.net/">WEBSITE</a>
  </h4>
</div>

<br />

<!-- Table of Contents -->
# :notebook_with_decorative_cover: Table of Contents

- [About the Project](#star2-about-the-project)
  * [Pictures](#camera-Pictures)
  * [Features](#dart-features)
- [Getting Started](#toolbox-getting-started)
  * [Schematic](#electric_plug-Schematic)
  * [Installation](#gear-installation)
- [Usage](#eyes-usage)
- [Contributing](#wave-contributing)
- [License](#warning-license)
- [Contact](#handshake-contact)

  

<!-- About the Project -->
## :star2: About the Project
In this project, we will control a simple robot by using voice commands using the XIAO nRF52840 Sense that has a built-in microphone. In this project, we use the micro_speech library, and the received commands are displayed on the old screen.


<!-- Pictures -->
### :camera: Pictures

<div align="center"> 
  <img src="https://user-images.githubusercontent.com/62047147/198869252-0cd978b5-6936-49f4-a0eb-8802ec8c543f.jpg" alt="screenshot" />
</div>


<!-- Features -->
### :dart: Features

- 4 Different Voice Commands
- Show all received commands on Oled Display

<!-- Getting Started -->
## 	:toolbox: Getting Started

We will use XIAO nRF52840 Sense as a processor. and we will add an OLED display to show received commands. Also with the Help of the DRV8833 Dual Motor Driver Module, we were able to control our DC Motors as Voice Commands were received.

- XIAO nRF52840 Sense
- DRV8833 Dual Motor Driver
- Oled 0.96 SSD1306

<!-- Schematic -->
### :electric_plug: Schematic
Make the connections according to the table and schematic below.

* XIAO nRF52840 and DRV8833.

We Should Connect STBY pin to VCC pin.

| XIAO nRF52840 | DRV8833 |  
| ----   | -----|
| 1   | AIN1|
| 2   | AIN2|
| 10  | BIN1|
| 9   | BIN2|
| 5V  | Vm  |
| GND | GND |


* XIAO nRF52840 and OLED display.

| XIAO nRF52840 | Oled 0.96|
| ----   | -----|
| 5  | SCK |
| 4  | SDA |
| 5V | VDD |
| GND | GND |

 
* Complete Schematic

<img src="https://user-images.githubusercontent.com/62047147/198869760-02b3f2b8-ce71-41f1-98a1-4fd1527de672.png" alt="screenshot" width="800" height="auto" />


<!-- Installation -->
### :gear: Installation

Before uploading the code you need to install the required library in Arduino IDE. Follow these steps:

- Follow this path Sketch> Include Library> Manage Libraries
- Search for Adafruit SSD1306
- Install the library

-Then search for the “GFX” and install it also.
   
<!-- Usage -->
## :eyes: Usage

After completing all the steps, the robot moves by receiving voice messages and the received messages are displayed on the screen.

<!-- Contributing -->
## :wave: Contributing

<a href="https://github.com/cifertech/2.4-GHz-band-Scanner/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=cifertech/2.4-GHz-band-Scanner" />
</a>


<!-- License -->
## :warning: License

Distributed under the MIT License. See LICENSE.txt for more information.


<!-- Contact -->
## :handshake: Contact

CiferTech - [@twitter](https://twitter.com/cifertech1) - CiferTech@gmali.com

Project Link: [https://github.com/cifertech/XIAO-ROBOT](https://github.com/cifertech/XIAO-ROBOT)

<!-- Acknowledgments -->
## :gem: Acknowledgements 

 - The main code for voice recognition and analysis is related to the [TensorFlow Lite](https://github.com/lakshanthad/tflite-micro-arduino-examples).
