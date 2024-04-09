# 📋 Test Plan


<details>
<summary>📖 Table of contents</summary>

- [📚 Glossary](#glossary)
- [🚀 Introduction](#introduction)
- [🎯 Project overview](#project-overview)
- [🎮 Testing strategy](#testing-strategy)
- [🔍 Testing scope](#testing-scope)
- [⏰ Testing schedule](#testing-schedule)
- [📝 Test cases](#test-cases)
- [🛠️ Testing tools](#testing-tools)
- [🐞 Defect tracking](#defect-tracking)
</details>

---

| Term | Definition |
| --- | --- |
| 🔍 Smoke test | A smoke test is a type of software testing that comprises a non-exhaustive set of tests that aim to ensure that the most important functions work. |
| 🧪 Functional test | Functional testing is a quality assurance (QA) process and a type of black-box testing that bases its test cases on the specifications of the software component under test. |
| 🔁 Regression test | Regression testing is a type of software testing that seeks to uncover new software bugs, or regressions, in existing functional and non-functional areas of a system after changes such as enhancements, patches, or configuration changes. |
| 🔬 Test case | A test case is a set of conditions or variables under which a tester will determine whether an application, software system, or one of its features is working as it was originally established for it to do. |
| 🧩 Unit test | A unit test is a method of testing individual components or units of code in isolation to ensure their correctness and functionality within a software system. |
| 📶 Bluetooth Low Energy (BLE) | A wireless communication technology designed for short-range communication between devices with low power consumption. |
| 📱 Near Field Communication (NFC) | A set of communication protocols that enable two electronic devices, such as a smartphone and a payment terminal, to establish communication by bringing them within close proximity. |
| 🛡️ Data integrity | The accuracy, consistency, and reliability of data stored and transmitted within a system, ensuring that data remains unchanged and uncorrupted during storage and transfer. |
| 📈 Scalability testing | The process of evaluating a system's ability to handle increasing workload or user demand by adding resources, such as CPU, memory, or storage, without sacrificing performance. |
| 🤝 Integration testing | Testing performed to verify the interactions and interfaces between different components or modules of a system to ensure that they work together as intended. |


## 🚀 Introduction

This document outlines the test plan for the SportShield project, an anti-theft device designed for skis and snowboard only at the moment. The purpose of this test plan is to test the code of the software engineers to make sure it allows for less battery consumption, without any error. This project has been given to us by Coris Innovation in collaboration with ALGOSUP, who are therefore the stakeholders.

## 🎯 Project overview

SportShield is an anti-theft device equipped with sensors and actuators to detect movement, activate an alarm, and notify the owner, it is linked with a mobile application, where the user can deactivate the alarm and manage settings. The device targets individual users of medium to high-end skis and snowboards initially, with plans to expand to other sports equipment and gear.

## 🎮 Testing strategy

The testing strategy for the SportShield project involves comprehensive testing of both hardware and software components. This includes functional testing, performance testing, security testing, and reliability testing. Testing will be conducted manually and through automated tests where applicable.

## 🔍 Testing scope

The testing scope includes:
- Activation and deactivation of the anti-theft alarm via Bluetooth
- Unlocking the device via Bluetooth and NFC
- Movement detection and alarm activation
- GPS localization and notification transmission
- Battery consumption
- Mobile app functionalities
- Data integrity and privacy
- Localization and internationalization
- Error handling and recovery
- Scalability and performance
- Integration testing

## ⏰ Testing schedule

The testing schedule will be determined based on the development progress. Testing phases will occur concurrently with development milestones to ensure timely detection and resolution of issues. The initial testing phase is expected to start on 03/25 and end on 04/10.

## 📝 Test cases

Test cases will cover various scenarios to validate the functionality and reliability of the SportShield device and mobile app. Each test case will include:
- Test case ID
- Test case name
- Test case description
- Test steps
- Expected result
- Actual result
- Status
- Priority
- Assigned to

And you will be able to find all the test cases in this [document](test-cases.md).

## 🛠️ Testing tools

The following tools will be used for testing:
- Hardware: SportShield device prototype, compatible smartphones, and different computers for testing the code, which are:
    
- [MacBook Air 2020](https://www.apple.com/fr/macbook-air-m1/)
    - 13.3 inch (2560 x 1600)
    - macOS Ventura 13.0
    - Apple M1 Chip

- [Lenovo Thinkbook 14](https://pcsupport.lenovo.com/us/en/products/laptops-and-netbooks/thinkbook-series/thinkbook-14-iil/20sl)
  - Windows 11 Pro
  - 14 inch (1920 x 1080)
  - Processor: Intel(R) Core(TM) i7-1065G7 CPU @ 1.30GHz
  - RAM: 16.0 GB
  - System type: 64-bit operating system, x64-based processor
  
- [ThinkBook 14 G4 IAP](https://psref.lenovo.com/syspool/Sys/PDF/ThinkBook/ThinkBook_14_G4_IAP/ThinkBook_14_G4_IAP_Spec.pdf)
  - Windows 11 Pro
  - 14 inch (1920 x 1080)
  - Processor: 12th Gen Intel(R) Core(TM) i7-1255U   1.70 GHz
  - RAM: 16.0 GB
  - System type: 64-bit operating system, x64-based processor

- Software: Mobile app, Arduino IDE for embedded software testing
- Communication tools for collaboration and issue tracking: GitHub, Slack and Trello.

## 🐞 Defect tracking 

We will use GitHub Issues to track the defects of the software and the documentation. We will create a new issue for each defect that we find during the testing of the software and the reviewing of the documentation. Every issue will be labeled with the `bug` for the software and with `documentation` otherwise and will be assigned to the person concerned who will fix the defect. They will be provided to the individual with a clear description of the issue, the expected result and relevant hints if necessary. Finally we will indicate its priority level with a scale from `low` to `critical`.

