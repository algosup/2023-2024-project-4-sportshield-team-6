# Functional Specification Document | Team 6

--- 

<details>
<summary> Table of Contents </summary>

- [Functional Specification Document | Team 6](#functional-specification-document--team-6)
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
    - [Testing](#testing)

</details>

---

## Context

### Problem

This project was presented to us by [Coris Innovation](https://www.corisinnovation.com) via [ALGOSUP](https://algosup.com/). Its objective is for us to improve Coris's work on their new project, SportShield.

SportShield is a device intended to help customers secure their skis or snowboard when they are not using them (i.e., during lunchtime). 
The product locks the object(s) in place using a cable for physical security (for now). That cable will lock itself to protect from unwinding when locked. 
The product is also equipped with an alarm system for when there is movement (i.e., a theft attempt). 
This is linked together via a mobile app that allows you to lock/unlock the device, stop the alarm, or check the device's position on a map.

### Target and Stakeholders

This document is addressed to the Tech Lead, the Software Engineer, the Quality Assurance, and the stakeholders, who are the client (Coris Innovation) and ALGOSUP (Franck). This document will describe the project's expected specifications and will act as a guideline for the developers.

### Competition

We identified one competitor of SportShield, SkiKey: 
They provide a key to lock skis/snowboard and variants of those two. The key serves to lock the skis/snowboard in place in a free-standing rack that the company also produces.

## Scope

### In Scope

 - Battery consumption management,
   - Improved energy efficiency,
   - Management of low-battery situations,
   - Increase of the battery lifespan,
 - Device management with NFC,
 - Alarm management and simultaneous actions,
   - Possibility to stop the alarm at any time,
   - The product can ring and still send HTTP notification to the server,
 - Security issues,
   - Increased security level to connect to the key feature of the system.

### Out of Scope

 - Improve the Hardware of the product,
 - Improve the protective case of the product.

## Use Case

### Personas

## Requirements

Here are the requirements of this project and their criticality (importance/order of implementation)
| Requirement | Criticality |
| :-------------| :-----: |
| Shock detection | Highest |
| Locking/Unlocking | Highest |
| Alarm | High |
| Shock Notification | High |
| GNSS Position | Medium |

### Deadlines

The deadlines for this project are as follows:

| Deliverable | Date |
|:-------------|:----------:|
| Functional | 18/03 5pm |
| Technical | 26/03 5pm |
| Test Plan | 10/04 5pm |
| User Manual | 10/04 5pm |
| Code | 10/04 5pm|

### Testing

For testing, we will test all the functionalities of the product. We will use the code provided to us by Coris Innovation as a base for both our development and our testing.

As we are adding our work on top of another people's one, we must respect the already in-place conventions.