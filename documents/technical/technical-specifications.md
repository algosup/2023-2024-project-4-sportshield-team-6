
# Technical specification - Team 6 

### [Coris innovation](https://www.corisinnovation.com) Sport-Shield Project given by [ALGOSUP](https://www.algosup.com)

<details>
<summary>Details</summary>

- Author: Ian LAURENT
- Created on the 13th March 2024
- Reviewers: 
    - Guillaume DERAMCHI (Quality Assurance)
    - Evan UHRING (Project Manager)
- Last updated: 26th March 2024
</details>

## Technical Specification Approval

|**Name**               |**Role**           |**Signature**  |**Date**  |
|-----------------------|-------------------|---------------|----------|
| Evan UHRING           | Project Manager   |      ✅       |03/26/2024|
| Jason GROSSO          | Program Manager   |      ✅       |03/26/2024|
| Ian LAURENT           | Tech Lead         |      ✅       |03/26/2024|
| David CUAHONTE CUEVAS | Technical Writer  |      ✅       |03/26/2024|
| Gaël MALVAR           | Software Engineer |               |          |
| Guillaume DERAMCHI    | Quality Assurance |      ✅       |03/26/2024|

## Table of Contents

1. Introduction to the project
    - Deadlines
    - Materials
    - Electronics
    - Libaries
        - Main libaries used
        - IDE

2. Provided documents

3. Goals / Product technical requirements
    - Product requirements in the form of user stories
    - Technical requirements
4. Non-goals or out of scope
5. Future goals
6. Assumptions
7. Solutions
    - Current or existing solution / design
    - Suggested or proposed solution / design
    - Test plan layout
    - Monitoring and alerting plan
8. Further considerations
    - Alternate solutions / designs
9. Success evaluation
    - Performance impact
    - Testing metrics
10. Work flow
    - Prioritization 
    - Milestones
    - Testing methods / Issue declaration
11. Glossary / Terminalogy
12. References
13. Acknowledgements
14. Legal

---
---


## Introduction

This project was given to us on March 11th 2024 as a school project with the task to optimise the code to be able to extend the battery life and reduce as much as possible the battery consumption. 
As for the device, it consists of an anti-theft device in the sport environment. It will be able to ring and emit a sound if movement is detected. It is equiped with an Arduino chip, and other components such as the movement sensor, a SIM module with a 2G SIM card, an antenna, a buzzer and finally a battery. The locking mechanism will work by using an electromagnet. 
You will find in this document all the specifications such as the voltage of each component in the **Electronics** section.

## Deadlines

These deadlines were given by Franck JEANNIN, a stakeholder of the project. You will find the whole list of the stakeholders in the **[Stakeholders](#stakeholders)** section.
- Functional 18/3 5pm
- Technical 26/3 5pm
- Test plan 10/4 5pm
- User Manual 10/4 5pm
- Code 10/4 5pm

## Materials
### Electronics
We were given a prototype of the product to be able to work on it. Here are the specifications of the components that were given by the client. 

|Image|Name|Dimensions|Description|Role|
|:-|:-|:-|:-|:-|
|<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Xiao%20BLE%20Sense%20nrf52840-Img.jpg" height="100">|Xiao BLE Sense nrf52840|2 x 2 x 0,5 cm | It is comparable to the processor | Connects the USB C to the computer to import the code file.|
| <img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/GNSS%20PA1010D-Img.png" height="100">|GNSS PA1010D | 2,5 x 2,5 x 1 cm | With antenna integration |This will allow to detect the movements of the board.
|<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/GSM%3A2G%20SIM800L%20Module-Img.jpg" height="100"> |GSM/2G SIM800L Module|2,2 x 1,8 x 0,5 cm | SIM card holder with 2G | This module will allow the board to connect to the 2G and send the location coordinates.
|<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Electromagnet-Img.png" height="100">|Electromagnet|2,7 x 1,6 x 1,3 cm | 12V and 500mA electromagnet| This will allow to lock and unlock the system with the program.| 
| <img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Piezoelectric-buzzer-Img.png" height="100">|Piezoelectric buzzer|1,5cm diameter |12V with oscillator circuit control|This buzzer will allow to emit a sound ranging from 90db to 100db.
|<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Lithium-Polymer%20battery-Img.png" height="100">|Lithium-Polymer battery|5,1 x 3,5 x 0,6 cm | 3,7V 1100mAh and 4.1Wh lithium battery | Power source of the board and the electromagnet.|
|<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/NFC-antenna-Img.png" height="100">|NFC antenna| 5,5 x 4,5 x 0,017cm|13,56Mhz frequency NFC antenna| This will allow the final user to use NFC technology to interact with the device.
|| USB type A to USB type C |10cm |10A connector| Will allow to connect for recharging and uploading code file.

These documents above were provided to our team to guide us and to allow the team to understand the physical architecture of the board.

## Libraries

In the domain of C++ programming, a library represents the core element, housing a curated collection of precompiled code modules or functions that furnish developers with reusable software components. These libraries encompass a diverse array of functionalities, spanning algorithms, data structures, utilities, and more, thereby offering indispensable resources for incorporation into various projects. Leveraging libraries affords developers the opportunity to circumvent redundant coding efforts, optimize development processes, and promote modular design principles within their software endeavors. Additionally, libraries often abstract complex functionalities behind streamlined interfaces, facilitating their seamless adoption and integration. Notably, standard libraries, exemplified by the C++ Standard Library, assume a central role by furnishing a comprehensive suite of functionalities aligned with standardized specifications, ensuring cross-platform compatibility and interoperability across heterogeneous environments. Ultimately, libraries serve as cornerstones of C++ programming, enabling practitioners to achieve code reusability, modularity, and the construction of robust and efficient software solutions.

### Main libraries used
- NRF52_MBED_TimerInterrupt V1.4.1
- ArduinoBLE v1.3.6
- Adafruit GPS Libary V1.7.4
- Sim800L http connector V1.14.0
- Seeed Arduino LSM6DS3 V2.0.3
- OneWire V2.3.7

### IDE
An Integrated Development Environment (IDE) is a software application that provides comprehensive facilities to programmers for software development. IDEs typically include features such as code editors, compilers or interpreters, build automation tools, debuggers, and project management capabilities, all integrated into a single cohesive environment. These tools are designed to enhance developer productivity by providing a unified workspace where programmers can write, edit, compile, debug, and deploy their code efficiently. IDEs are available for various programming languages and platforms, catering to the specific needs of developers across different software development domains. Popular examples of IDEs include Visual Studio, Eclipse, IntelliJ IDEA, and Xcode.

The working environnement for this project is **[Arduino IDE 2.3.2](https://www.arduino.cc/en/software)**

### App

There is a designated mobile app that will allow the end user to control the final product on his device (e.g. Phone). This app's name is SportShield curated by Coris Innovation. This app controls the lock and unlock function by emitting frequencies to the antenna via Bluetooth technology. This app also allows the user to see the precise location of the lock with the GPS location on the board. NFC technology is planned to be implemented after release by Coris Innovation, they plan on making the lock and unlock system possible by tapping the NFC antenna with the user's device or badge to unlock it. 

Here is the APK link to download the unreleased app: [Download]()--michel--

## Provided documents

[Specifications on the SIM module (GSM/2G SIM800L Module)](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/SIM800L-SIMCom.pdf)

---

[Specifications on antenna module(GNSS PA1010D)](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/CD-PA1010D-Datasheet-v.02%20(2).pdf)

---

Specifications document on Xiao BLE Sense nrf52840 module:
- [nrf52840 specific product specifications](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/nRF52840_PS_v1.5.pdf)

- [Board scheme](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/Seeed-Studio-XIAO-nRF52840-Sense-v1.1.pdf)

---

[Battery specifications document](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/Batterie_LP603449.pdf)


## Goals / Product technical requirements
### Product requirements in the form of user stories

Optimisation was the main task of the assignment. Other considerations such as library optimisation and board power optimisation will be conceivable however the team must not lose scope of the principle task. 

### Technical requirements
**Optimisation**: Optimisation is key here, where as our main focus will be on the optimisation of the already existing code. The detection of the movements will have to be optimised to be precise but also neglecting the small movements caused by other factors then it's primary function of protecting from theft.

**Reliability**: Reliability will be the second requirement due to the product being a lock for sport equipement. The system has to be reliable with no flaws in the system. The movements and the location will have to be reliable for the final user to be able to locate and be notified when a movement is detected. 

**Performance**: At last, performance will need to be taken into consideration for the product to be accurate. GPS location will have to be precise to locate the device in case of theft or a lost of the device. The detection of movement has to be correct and will have to detect every movement taking into account the meteorological conditions that the device can face such as storms, strong winds, and snow.

## Non-goals or out of scope

Changing the physical board is part of the non-goals, the team will stay focused in working on the software and not the hardware, due to the demand of the client to only optimise the code the team will focus its attention to the software first. Once this task will be terminated it will be conceivable to propose to the client a new prototype.
## Future goals

## Assumptions
The product will be fully functional with GPS location precisely pinned, and the movement detection will be flawless with the code being fully optimised to extend its battery life. The battery life will be extended to one week with a constant use of 2 hours per day. This will allow us to meet the expectations of the client. 
## Solutions 

The solution that the team is considering is to minimise the constant GPS location search and allow it to activate only when the device detects a movement. In addition, allowing a range of tolerance in the detection of the movement which will allow to consume a lot less power but also avoid unwanted alerts caused by other factors such as wind. 
In complementary to the proposed solution, the team will propose to add an element onto the existing protoype to maximise battery life and avoid unwanted power consumption. 
An alternative solution would be to upgrade the current battery to one with a bigger capacity to allow the battery to last even longer, taking into account the cost of production we wouldn't want to higher that. Which is why it would be the last solution if after the code optimisation the battery life doesn't meet the customer's demands. 
Adding materials that will autoregulate in terms of temperature is also a proposition from our team, due to the extreme conditions that the final user will take the device to. The device should be able to resist to extreme cold and hot temperatures without affecting its performance, which is why materials such as a TRM[^1] is an aspect to consider in the design.

### Current or existing solution / Design

![img](../pictures/Electronics.png)

As shown above, this is the prototype that we have received to work on. It contains all the main components.

[Source code](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/tree/Dev/SS_05-03_anglais-batterycontrol)

The source code linked above was given by <u>Corris Innovation</u>, and is currently not optimised.

[Developed code](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/tree/Dev/SS_05-03_anglais-batterycontrol)

Above is the optimised code from the source code that will be uploaded to the board and will run on. 

### Suggested or proposed solution / Design


### Test plan layout

The quality assurance team wrote an organised test plan for ensuring that our work functions as intended, to access it, click [here](../quality-assurance/test-plan.md).

### Monitoring and alerting plan
We will use GitHub Issue for tracking defects, more details in the test plan as well.

## Further considerations
One major consideration for the physical component would be to add an electrical condensator connected to the board, to the electromagnet. Due to the power being converted in the current display, the electromagnent doesn't receive enough power to be activated. 
This leads to performance issues and more importantly to reliability issues.

The battery has also to be considered to be changed to a higher voltage battery, the current provided by the battery doesn't have the capabilities to activate the electromagnet. 

### Alternative solutions / designs

In the case of the code optimisation is not meeting the clients satisfaction, we are considering to propose change the battery to a higher autonomy battery, and adding an electrical condensator in the circuit.

## Success evaluation

The code will be fully optimised, assuming that the electromagnet is fully functional and that the battery will be able to provide the electromagnet with the right amount of power for it to be actionned. 

### Performance impact 
Due to the low power that the electromagnent will receive, it will have a major impact on performance but also on reliability. The alarm system will be activated, however the lock system could be faulty leading to an important vulnerability of the device getting stolen.

### Testing (metrics)

Voltimeter and other unit tests will be done to assure that the results coming from the tests ressemble to the expected result. 

## Work flow

Our team is composed with a project manager, a program manager, a tech leader, a quality assurance, a technical writer, and a software engineer. This configuration allows the team to have a specific work flow where as all the steps of the project will have to be validated by the quality assurance and the project manager. This allows to keep the workflow going, and to assure an good quality outcome.

### Prioritisation
- Testing the protoype: Understanding the equipment we will have to work with is the first step.
- Initialisation: In this step, the team will run the provided code on the hardware to test one by one the different modules of the prototype.
- Reviwing: Understanding the provided code.
- Targeting: Finding the eventual flaws in the code that leads to an unoptimised battery consumption.
- Solving: Finding ways to optimise the code after detecting the flaws in the code.
- Implementation: Implementing new features to the code and other functions that could help it to respond to the client's needs.
- Presentation: Presenting to the client the final work detailing every aspect that was tweeked and added.

### Milestones 
| Position of step | Name | Description |
| -- | -- | -- |
| 1 | Alarm ringing and notifying | The alarm has to continue ringing when sending notifications to the user |
| 2 | Alarm stop at will | The user will be capable of stopping the alarm at will, without having to wait the end of the ringing |
| 3 | Battery efficiency | The product will use more efficiently the power from the battery to last longer |
| 4 | Battery lifespan | The product will have limitations for the battery charge to increase the battery lifespan |
| 5 | Low battery management | The product will have security capabilities when its battery is too low, so the user can still take his skis without the product locked on them |
| 6 | NFC | The user will be able to use the NFC in addition to the bluetooth to connect the product to his phone, to lock or unlock and activate or deactivate the product |

--

### Testing methods / Issue declaration 
The details of the different test methods and issue declaration can be found in the [test plan](../quality-assurance/test-plan.md).

## Stakeholders

The are two principle stakeholders for this project:
<details>
<summary>ALGOSUP International Software Development School</summary>

- **Franck JEANNIN** : Co-founder of ALGOSUP International Software Development School
- **Natacha BOEZ** : Co-founder of ALGOSUP International Software Development School
- **Éric LARCHEVÊQUE** : Co-founder of ALGOSUP International Software Development School
</details>

<details>
<summary>Coris Innovation</summary>

- **Florent ANON** : Representative of Coris innovation / Innovation Lab Manager.
</details>

## Glossary / Terminalogy 

[^1]: A substance that undergoes phase transition at a specific temperature, which enables it to absorb and release latent heat when isothermal conditions are altered.

## References
<u>Arduino IDE documentation:</u>
- [Software installation.](https://docs.arduino.cc/software/ide-v2/tutorials/getting-started/ide-v2-downloading-and-installing/)
- [Board package installation.](https://docs.arduino.cc/software/ide-v2/tutorials/ide-v2-board-manager/)
- [Installing libaries.](https://docs.arduino.cc/software/ide-v2/tutorials/ide-v2-installing-a-library/)
- [Understanding Aduino IDE.](https://docs.arduino.cc/software/ide-v2/tutorials/getting-started-ide-v2/)

<u>Getting started with Seeed Studio XIAO nRF52840 (Sense):</u>
- [Full documentation on installing the board correctly.](https://wiki.seeedstudio.com/XIAO_BLE/)

<u>Documentation explaining NFC technology:</u>
- [What is NFC.](https://www.raypcb.com/nfc-antenna/)

## Acknowledgements
We wish to express our sincere appreciation to ALGOSUP International Software Development School and Coris Innovation for their pivotal role in the development of this technical specifications documents. Their profound expertise, steadfast guidance, and collaborative spirit have profoundly enriched the conceptualisation and refinement of the project, ensuring its adherence to rigorous industry standards and best practices. The partnership with ALGOSUP International Software Development School and Coris Innovation has been instrumental in navigating intricate technical challenges and fostering innovative solutions to effectively meet the project's objectives. Their unwavering commitment and invaluable contributions have been indispensable in propelling the project towards its successful fruition.


<p align="center">
<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/65648d5d98f6814022b9474a_6e5ca96fcf317623caec20ca96892327.png" height="100">
</p>
<p align="center">
<img src="https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/ALGOSUP-logo.png" height="100" >
</p>


## Legal 

All intellectual property rights, including copyrights, patents, and proprietary information, associated with the development of these technical specifications for educational purposes and the prototype, are hereby acknowledged to belong solely to ALGOSUP International Software Development School and Coris Innovation. This legal acknowledgment confirms their exclusive ownership of the concepts, methodologies, algorithms, and any related documentation contained within the specifications. It is noted that certain information contained herein may be sensitive or proprietary to ALGOSUP International Software Development School and Coris Innovation and may not be suitable for public dissemination. Any unauthorised use, reproduction, or distribution of this intellectual property without explicit authorisation from ALGOSUP International Software Development School and Coris Innovation is strictly prohibited and may result in legal action.

