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
  - [Use Cases](#use-cases)
      - [Use case name: Locking skis/snowboard with SportShield](#use-case-name-locking-skissnowboard-with-sportshield)
      - [Use case name: Storage in a Ski Resort's Equipment Room with SportShield](#use-case-name-storage-in-a-ski-resorts-equipment-room-with-sportshield)
      - [Use case name: Transportation Security with SportShield](#use-case-name-transportation-security-with-sportshield)
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

---

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

## Use Cases

---

#### Use case name: Locking skis/snowboard with SportShield

**Description:** A skier or snowboarder uses SportShield to secure their equipment when not in use, providing security and peace of mind.

**Actor:** Skier or snowboarder

**Stakeholder:** Ski resort management, skier or snowboarder

**Primary actor:** Skier or snowboarder

**Preconditions:**
- The skis or snowboard are not in use and need to be secured.
- The skis or snowboard are equipped with SportShield.
- The user has access to their smartphone with the SportShield application installed.

**Triggers:** The skier or snowboarder finishes using their equipment and needs to secure it before leaving the area.

**Basic flow:**
1. The skier or snowboarder finishes their run on the slopes and reaches a designated area for equipment storage.
2. The user retrieves their smartphone and opens the SportShield application.
3. The user selects the option to lock their skis or snowboard.
4. The user attaches the SportShield to their equipment and a fixed structure, such as a rack or post.
5. The user confirms the lock action in the SportShield application.
6. The SportShield secures the equipment, providing a visual indication of the locked status.
7. The skier or snowboarder leaves the area with peace of mind, knowing their equipment is securely locked.

**Alternative path:**
- If the user encounters any issues with SportShield (e.g., low battery, connectivity issues), they can troubleshoot by checking the lock's status in the application and following any on-screen instructions for resolution.
- If the user forgets to lock their equipment before leaving the area, they can remotely lock it using the SportShield application from wherever they are located.
- If the user mistakenly locks the equipment but needs to access it again, they can use the SportShield application to remotely unlock the cable and retrieve their skis or snowboard.

#### Use case name: Storage in a Ski Resort's Equipment Room with SportShield  

**Description:** Skiers and snowboarders staying at a ski resort use SportShield to secure their equipment in the resort's equipment room overnight, preventing theft and ensuring gear remains safe and secure while they rest.  

**Actor:** Skier or snowboarder  

**Stakeholder:** Ski resort management, skiers/snowboarders  

**Primary actor:** Skier or snowboarder  

**Preconditions:**
- Skier or snowboarder is staying at a ski resort.
- The skis or snowboard need to be securely stored overnight.
- The skis or snowboard are equipped with SportShield.
- A designated rack or storage area is available in the resort's equipment room.  

**Triggers:** Skier or snowboarder finishes skiing or snowboarding for the day and wants to securely store their equipment overnight.  

**Basic flow:**
1. The skier or snowboarder locates the equipment room designated for gear storage in the ski resort.
2. The user retrieves their smartphone and opens the SportShield application.
3. The user selects the option to lock their skis or snowboard.
4. The user attaches the SportShield to their equipment and a designated rack or storage area in the equipment room.
5. The user confirms the lock action in the SportShield application.
6. The SportShield secures the equipment, providing a visual indication of the locked status.
7. The skier or snowboarder rests or stays overnight, knowing that their equipment is securely 

**Alternative path:**
- If the user encounters any issues with SportShield (e.g., low battery, connectivity issues), they can troubleshoot by checking the lock's status in the application and following any on-screen instructions for resolution.
- If the designated rack or storage area is unavailable or occupied, the user can explore alternative options for securing their equipment, such as asking resort staff for assistance or locating another designated area for equipment storage.

#### Use case name: Transportation Security with SportShield  

**Description:** Skiers and snowboarders traveling to and from the mountain use SportShield to secure their equipment during transit, preventing theft and ensuring gear remains safe and secure.  

**Actor:** Skier or snowboarder  

**Stakeholder:** Ski resort management, skiers/snowboarders  

**Primary actor:** Skier or snowboarder  

**Preconditions:**
- Skier or snowboarder is traveling to or from the mountain.
- The skis or snowboard need to be securely transported.
- The skis or snowboard are equipped with SportShield.
- A roof rack, ski rack, or cargo area is available in the vehicle for securing the equipment.  

**Triggers:** Skier or snowboarder begins or ends their trip to the mountain and wants to secure their equipment during transit.  

**Basic flow:**
1. The skier or snowboarder prepares to transport their equipment to or from the mountain.
2. The user retrieves their smartphone and opens the SportShield application.
3. The user selects the option to lock their skis or snowboard.
4. The user attaches the SportShield to their equipment and a roof rack, ski rack, or cargo area in the vehicle.
5. The user confirms the lock action in the SportShield application.
6. The SportShield secures the equipment, providing a visual indication of the locked status.
7. The skier or snowboarder travels to or from the mountain, knowing that their equipment is securely locked and protected during transit.  

**Alternative path:**
- If the user encounters any issues with SportShield (e.g., low battery, connectivity issues), they can troubleshoot by checking the lock's status in the application and following any on-screen instructions for resolution.
- If the designated area for securing the equipment is unavailable or occupied, the user can explore alternative options for securing their equipment, such as using additional straps or finding another suitable location within the vehicle.

### Personas

## Requirements

---

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

---