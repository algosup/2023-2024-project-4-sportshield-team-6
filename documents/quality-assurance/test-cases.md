## Test Cases

---

### Order of priority

| Order | Name |    
|---|---|   
| 1 | Critical |    
| 2 | High |    
| 3 | Medium |      
| 4 | Low |     

---

- Test case ID: 1
- Test case name: Test the movement detection algorithm
- Test case description: This test case verifies the correct detection of slight and significant movements.
- Test steps:
    1. Perform slight movements.
    2. Perform significant movements.
- Expected result: The movement detection algorithm should correctly detect the movements.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If the movement detection fails, restart the system and retest.

---

- Test case ID: 2
- Test case name: Test the alarm activation algorithm
- Test case description: This test case verifies the correct activation and deactivation of the alarm.
- Test steps:
    1. Trigger significant movements.
    2. Wait for the specified time period.
- Expected result: The alarm should activate upon detecting significant movements and deactivate after the specified time period.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If the alarm activation fails, reset the alarm system and retest.

---

- Test case ID: 3
- Test case name: Test Bluetooth connectivity
- Test case description: This test case verifies the pairing, data transmission, and reconnection between the SportShield device and the mobile app.
- Test steps:
    1. Pair the SportShield device with the mobile app.
    2. Test data transmission between the device and the app.
    3. Test reconnection after Bluetooth disconnection.
- Expected result: The SportShield device should successfully pair with the mobile app, transmit data, and reconnect after disconnection.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If Bluetooth connectivity fails, restart Bluetooth on both devices and retest.

---

- Test case ID: 4
- Test case name: Test battery management
- Test case description: This test case verifies the sleep functionality.
- Test steps:
    1. Test sleep functionality.
- Expected result: The sleep functionality should work as expected, so the hardware supposed to not be working when sleep mode is activated should not, and when the active hardware detects something, it should reactivate the hardware put in sleep mode.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: High
- Assigned to: QA
- Recovery steps: If battery management fails, recharge the device and retest.

---

- Test case ID: 5
- Test case name: Test integration between movement detection and alarm activation
- Test case description: This test case verifies the integration between the movement detection algorithm and the alarm activation algorithm.
- Test steps:
    1. Trigger movements.
- Expected result: The alarm should activate correctly upon detecting movement, and there should be synchronization between the movement detection and alarm activation.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If integration fails, restart the system and retest.

---

- Test case ID: 6
- Test case name: Test battery performance
- Test case description: This test case evaluates the battery life, charging, and discharging behavior.
- Test steps:
    1. Evaluate battery life under different usage scenarios.
    2. Test battery charging and discharging behavior.
- Expected result: The battery should perform as expected in terms of life, charging, and discharging behavior, so it should last for 7 days, considering 6 hours activation mode + 18 hours in stand-by (not activated) mode per day, as well as cold conditions.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If battery performance is unsatisfactory, recharge the device and retest.

---

- Test case ID: 7
- Test case name: Usability testing of the mobile app
- Test case description: This test case evaluates the ease of use for activating/deactivating the alarm and unlocking the device via Bluetooth.
- Test steps:
    1. Open the mobile app.
    2. Locate and tap the button to activate the alarm.
    3. Verify the alarm activation.
    4. Deactivate the alarm using the app.
    5. Verify the alarm deactivation.
    6. Attempt to unlock the device via Bluetooth using the app.
    7. Verify successful device unlocking.
- Expected result:
    - Steps 2-3: The alarm should activate smoothly with a clear indication.
    - Steps 4-5: The alarm should deactivate smoothly with a clear indication.
    - Steps 6-7: The device should unlock seamlessly with a clear confirmation.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If usability issues arise, provide user training and retest.

---

- Test case ID: 8
- Test case name: Performance Testing
- Test case description: This test case evaluates the system's responsiveness.
- Test steps:
    1. Measure the response time of key functions such as alarm activation, device unlocking, and GPS localization.
- Expected result: The system should maintain acceptable response times under normal usage scenarios and demonstrate scalability to accommodate increased load.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: High
- Assigned to: QA
- Recovery steps: If response times are too slow, optimize system resources and retest.

