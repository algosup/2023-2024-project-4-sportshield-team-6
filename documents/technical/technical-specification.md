<<<<<<< Updated upstream
=======
# Technical specification - Team 6 

### [Coris innovation](https://www.corisinnovation.com) Sport-Shield Project givin by ALGOSUP [ALGOSUP](https://www.algosup.com)

Details: 
- Author: Ian LAURENT
- Created on the 13th March 2024
- Reviewers: 
    - Guillaume DERAMCHI (Quality Assurance)
    - Evan UHRING (Project Manager)
- Last updated: 25th March 2024


## Technical Specification Approval

|**Name**               |**Role**           |**Signature**  |**Date**  |
|-----------------------|-------------------|---------------|----------|
| Evan UHRING           | Project Manager   |               |          |
| Jason GROSSO          | Program Manager   |               |          |
| Ian Laurent           | Tech Lead         |               |          |
| David CUAHONTE CUEVAS | Technical Writer  |               |          |
| Gaël MALVAR           | Software Engineer |               |          |
| Guillaume DERAMCHI    | Quality Assurance |               |          |

## Table of Content

1. Introduction to the project
    - deadlines
    - Materials
    - Electronics
    - Libaries
        - Main libaries used
        - IDE

2. Provided documents

3. Goals / Product Technical Requirements
    - Product requirements in the form of user stories
    - Technical requirements
4. Non-Goals or Out of Scope
5. Future goals
6. Assumptions
7. Solutions
    - Current or Existing Solution / Design
    - Suggested or Proposed Solution / Design
    - Test Plan layout
    - Monitoring and Alerting Plan
8. Further considerations
    - Alternate Solutions / Designs
9. Success Evaluation
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


## Introduction

This project was given to us on March 11th 2024 as a school project with the task to obptimise the code to be able to extend the battery life and reduce as much as possibke the battery consuption. 
As for the device the device consists of a anti-theift device in the sports environment it will be able to ring and emit a sound if movement is detected. It is equiped with a arduino chip, and other componants such as the movement sensor, a sim module with a 2g sim card, an anthenna, the buzzer and finally the battery. The lock will be able to be locked with an electro-magnet. 
You will find in this document all the specifications such as the voltage of each componant in the **Electronics** section.

## Deadlines

These deadlines were givin by Franck JEANNIN a stakeholder of the project. You will find the whole list of the stakeholders in the "" section.
- Functional 18/3 5pm
- Technical 26/3 5pm
- Test plan 10/4 5pm
- User Manual 10/4 5pm
- Code 10/4 5pm

## Materials

### Electronics
We were givin a prototype of the product to be able to work on it, Here is the specification of the componants that were givin by the client. 

|Image|Name|Dimensions|Description|Role|
|:-|:-|:-|:-|:-|
|![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Xiao%20BLE%20Sense%20nrf52840-Img.jpg)|Xiao BLE Sense nrf52840|2 x 2 x 0,5 cm | | Connects the USB C to the computer to import the code file.|
| ![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/GNSS%20PA1010D-Img.png)|GNSS PA1010D | 2,5 x 2,5 x 1 cm | With antenna integration |This will allow to detect the movements of the board.
|![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/GNSS%20PA1010D-Img.png) |GSM/2G SIM800L Module|2,2 x 1,8 x 0,5 cm | Sim card holder with 2G | This module will allow the board to connect to the 2G and send the location coordinates.
|![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Electromagnet-Img.png)|Electromagnet|2,7 x 1,6 x 1,3 cm | 12V and 500mA electromagnet| This will allow to lock and unlock the system with the program.| 
|![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Piezoelectric-buzzer-Img.png)|Piezoelectric buzzer|1,5cm diameter |12V with oscillaor circut control|This buzzer will allow to emit a sound ranging from 90db to 100db.
|![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/Lithium-Polymer%20battery-Img.png)|Lithium-Polymer battery|5,1 x 3,5 x 0,6 cm | 3,7V 1100mAh and 4.1Wh lithium battery | Power source of the board and the electromagnet.|
|![Image](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/NFC-antenna-Img.png)|NFC antenna| 5,5 x 4,5 x 0,017cm|13,56Mhz frequency NFC antenna| This will allow the final user to use NFC technology to interact with the device.
|| USB type A to USB type C |10cm |10A connector| Will allow to connect for recharging and uploading code file.

These documents under was provided to our team to guide the team and for the team to understand the physical architecture of the board.

## Libaries

In the domain of C++ programming, a library represents a foundational element, housing a curated collection of precompiled code modules or functions that furnish developers with reusable software components. These libraries encompass a diverse array of functionalities, spanning algorithms, data structures, utilities, and more, thereby offering indispensable resources for incorporation into various projects. Leveraging libraries affords developers the opportunity to circumvent redundant coding efforts, optimize development processes, and promote modular design principles within their software endeavors. Additionally, libraries often abstract complex functionalities behind streamlined interfaces, facilitating their seamless adoption and integration. Notably, standard libraries, exemplified by the C++ Standard Library, assume a central role by furnishing a comprehensive suite of functionalities aligned with standardized specifications, ensuring cross-platform compatibility and interoperability across heterogeneous environments. Ultimately, libraries serve as cornerstones of C++ programming, enabling practitioners to achieve code reusability, modularity, and the construction of robust and efficient software solutions.

### Main libaries used
- NRF52_MBED_TimerInterrupt V1.4.1
- ArduinoBLE v1.3.6
- Adafruit GPS Libary V1.7.4
- Sim800L http connector V1.14.0
- Seeed Arduino LSM6DS3 V2.0.3
- OneWire V2.3.7

### IDE
An Integrated Development Environment (IDE) is a software application that provides comprehensive facilities to programmers for software development. IDEs typically include features such as code editors, compilers or interpreters, build automation tools, debuggers, and project management capabilities, all integrated into a single cohesive environment. These tools are designed to enhance developer productivity by providing a unified workspace where programmers can write, edit, compile, debug, and deploy their code efficiently. IDEs are available for various programming languages and platforms, catering to the specific needs of developers across different software development domains. Popular examples of IDEs include Visual Studio, Eclipse, IntelliJ IDEA, and Xcode.

The working environnement for this project is **Arduino IDE 2.3.2
"Link"**

## Provided documents

[Specification on the Sim module (GSM/2G SIM800L Module)](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/SIM800L-SIMCom.pdf)

---

[Specification on Anthenna module(GNSS PA1010D)](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/CD-PA1010D-Datasheet-v.02%20(2).pdf)

---

Specification document on Xiao BLE Sense nrf52840 module:
- [nrf52840 specific product specification](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/nRF52840_PS_v1.5.pdf)

- [Board scheme](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/Seeed-Studio-XIAO-nRF52840-Sense-v1.1.pdf)

---

[Battery Specification document](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/documentation/Batterie_LP603449.pdf)


## Goals / Product Technical Requirements
### Product requirements in the form of user stories

Optimisation was the main task of the asseignment, it being the key element to the success optimisation is the foundation to key success. Other considerations such as libary optimisation and board power optimisation will be conceivable however the team must not lose scope of the principle task. 

### Technical requirements
**Optimization**: Optimization is key here where as our main focus will be on the optimization of the already existing code. The detection of the movements will have to be optimized to be precise but also negleting the small movements caused by other factors then it's primary function of protecting from theift.

**Reliability**: Reliability will be the second requirement due to the product being a lock for sport equipement the system has to reliable with no flaws in the system. The movements and the location will have to reliable for the final user to be able to locate and be notified when a movement is detected. 

**Performance**: At last performance will need to be taken into consideration for the product to be accurate. GPS location will have to be precise to locate the device in case of theift or a lost of the devise. The detection of movement has to be correct and will have to detect every movement taking into account the meterological conditions that the device can face such as storms, strong winds, snow.

## Non-Goals or Out of Scope
--Product and technical requirements that will be disregarded

## Future Goals

## Assumptions
The product will be fully functional with GPS location precisly pinned, and the movement detection will be flawless with the code being fully optimized to extend it's battery life. The battery life will be extended to one week with a constant use of 2 hours per day. This will allow us to meet the standards of the client. 
## Solutions 
-- needs to be brought by Sofware developer
### Current or Existing Solution / Design

-- Add image of the product -- 

As shown above, this is the prototype that we have received to work on it contains all the main componants.

[Source code](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/tree/Dev/SS_05-03_anglais-batterycontrol)

The source code is linked above and was givin by <u>Corris Innovation</u> and is currently not optimised.

-- link to optimised code --

Above is the optimized code from the source code that will be uploaded to the board and will run on. 

### Suggested or Proposed Solution / Design


### Test Plan layout


### Monitoring and Alerting Plan

## Further considerations
One major consideration for the physical componant would be to add a electrical relay connected to the Battery, the board and the electromagnet. Due to the power being converted in the current display, the electromagnent doesn't receive enough power to be activated. 
This leads to performance issues and more importantly to reliability issues.

The battery has also to be considered to be changed to a higher voltage battery, the current provided battery doesn't have the capacities to action the electromagnent at this current moment. 
### Alternate Solutions / Designs

We propose to consider change the battery to a higher volatge battery, and adding a electrical relay in the circuit. 

## Success Evaluation

The code will be fully optimised assuming that the electromagnet is fully functional and that the battery will be able to provide the electromagnent with the right amount of power for it to be actionned. 

### Performance impact 
Due to the low power that the electromagnent will receive, it will have a major impact on performance but also oon reliability. The alarm system will be activated however the lock system could be faulty leading to an important vulnarability of the device getting stolen.

### Testing (metrics)
Voltimeter and other unit test will be done to assure that the results comming from the tests ressembles the expected result. 
## Work flow

### Prioritzation 
- Testing the protoype: Understanding the equipment we will have to work with is the first step.
- Initialisation: In this step the team will run the provided code on the hardware to test one by one the different modules of the prototype.
- Reviwing: Understanding the provided code.
- Targeting: Finding the eventual flaws in the code that leads to an unoptimised battery consumption.
- Solving: Finding ways to optimize the code after detecting the flaws in the code.
- Implementation: Implementing new features to the code and other functions that could help it to repond to the clients needs.
- Presentation: Presenting to the client the final work detailing every aspect that was tweeked and added.
### Milestones 
--EVAN--
### Testing methods / Issue declaration 
--Guillaume--
## Glossary / Terminalogy 

## References

## Acknowledgements
We wish to express our sincere appreciation to ALGOSUP and Coris Innovation for their pivotal role in the development of this technical specification. Their profound expertise, steadfast guidance, and collaborative spirit have profoundly enriched the conceptualization and refinement of the project, ensuring its adherence to rigorous industry standards and best practices. The partnership with ALGOSUP and Coris Innovation has been instrumental in navigating intricate technical challenges and fostering innovative solutions to effectively meet the project's objectives. Their unwavering commitment and invaluable contributions have been indispensable in propelling the project towards its successful fruition.

![Coris innovation logo](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/65648d5d98f6814022b9474a_6e5ca96fcf317623caec20ca96892327.png)
![ALGOSUPLOGO](https://github.com/algosup/2023-2024-project-4-sportshield-team-6/blob/Dev/documents/pictures/ALGOSUP-logo.png)

## Legal 

All intellectual property rights, including copyrights, patents, and proprietary information, associated with the development of this technical specification for educational purposes and the prototype, are hereby acknowledged to belong solely to ALGOSUP and Coris Innovation. This legal acknowledgment confirms their exclusive ownership of the concepts, methodologies, algorithms, and any related documentation contained within the specification. It is noted that certain information contained herein may be sensitive or proprietary to ALGOSUP and Coris Innovation and may not be suitable for public dissemination. Any unauthorized use, reproduction, or distribution of this intellectual property without explicit authorization from ALGOSUP and Coris Innovation is strictly prohibited and may result in legal action.
>>>>>>> Stashed changes
