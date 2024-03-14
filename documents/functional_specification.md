# Functional Specification Document  Team 6

--- 
 
<details>
<summary> Table of Contents </summary>

- [Functional Specification Document  Team 6](#functional-specification-document--team-6)
  - [Context](#context)
    - [Problem](#problem)
    - [Target and Stakeholders](#target-and-stakeholders)
    - [Competition](#competition)
  - [Scope](#scope)
    - [In Scope](#in-scope)
    - [Out of Scope](#out-of-scope)
  - [Use Case](#use-case)
    - [Personas](#personas)
  - [Requirements](#requirements)
    - [Deadlines](#deadlines)

</details>

---

## Context

### Problem

This project was presented to us by [Coris Innovation](https://www.corisinnovation.com)  via [ALGOSUP](https://algosup.com/), it's objective is for us to improve Coris's work on their new project, SportShield.

SportShield is a device intented to help customers secure their skis or snowboard when they are not using them (i.e. during lunchtime). 
The product lock the object(s) in place using a cable for physicla security(for now), that cable will lock itself to protect from unwinding when locked. 
The product is also equiped with an alarm system, when it mouvement (i.e. theft attempt). 
This is linked together via a mobile app that allows you to lock/unlock the device, stop the alarm or check the devices position on a map.

### Target and Stakeholders

This document is addressed to the Tech Lead, the Software Engineer, the Quality Assurance and the client (Coris Innovation). This document will describe the projects expected specifications and will act as a guideline for the developers.

### Competition

## Scope

### In Scope

 - Battery consumption management,
   - Improved energy effeciency,
   - Management of low-battery situations,
   - increase of the battery lifespan,
 - Device management with NFC,
 - Alarm management and simultaneous actions,
   - Possibility to stop the alarm at any time,
   - The product can ring and still send HTTP notification to the server,
 - Security issues,
   - Incresed security level to connect to the key feature of the system.

### Out of Scope

 - Improve the Hardware of the product,
 - Improve the protective case of the product.

## Use Case

### Personas

## Requirements

Here are the requirements of this project and their criticality(importance/order of implmentation)
| Requirement | Criticallity |
| :-------------| :-----: |
| Shock detection | Highest |
| Locking/Unlocking | Highest |
| Alarm | High |
| Shock Notification | High |
| GNSS Position | Medium |

### Deadlines

The dealines for this project are as such:

| Deliverable | Date |
|:-------------|:----------:|
| Functional | 18/03 5pm |
| Technical | 26/03 5pm |
| Test Plan | 10/04 5pm |
| User Manual | 10/04 5pm |
| Code | 10/04 5pm|
