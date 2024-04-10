## Test Cases

**Note: our software engineer didn't touch the code throughout the project, and let us uncertain if he would come back or not. So nothing has been implemented, and this has rubbed off on the completeness of the test cases. I apologize for that.**

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
- Expected result: The movement detection algorithm should correctly detect the movements, and emit sound more or less loud depending on the amplitude and the duration of the movement.
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
- Test case description: This test case evaluates the battery life.
- Test steps:
    1. Evaluate battery life under different usage scenarios.
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
- Test case name: Performance testing
- Test case description: This test case evaluates the system's responsiveness.
- Test steps:
    1. Measure the response time of key functions such as alarm activation, device unlocking, and GPS localization.
- Expected result: The system should maintain acceptable response times under normal usage scenarios and demonstrate scalability to accommodate increased load.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: High
- Assigned to: QA
- Recovery steps: If response times are too slow, optimize system resources and retest.

---

- Test case ID: 9
- Test case name: Sound level differences
- Test case description: This test case verifies that the 2 available alarm sound levels are different.
- Test steps:
    1. Perform slight movements.
    2. Perform major movements.
- Expected result: The sound emitted when slight movements are performed should be the 3-tone one. When major movements the sound emitted should be the 5-tone one.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Medium
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, optimize the code and retry.

---

- Test case ID: 10
- Test case name: Use of NFC
- Test case description: This test case verifies that the NFC is working properly on the SportShield device.
- Test steps:
    1. Use NFC to connect the phone with the device.
    2. Use NFC to unlock the device.
    3. Use NFC to lock the device.
- Expected result: The NFC should work appropriately, meaning that a phone with NFC implemented should connect and be able to lock and unlock the device at will.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Critical
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, optimize the code and retry.

---

- Test case ID: 11
- Test case name: Stop the alarm at will
- Test case description: This test case verifies that the alarm can be stopped whenever the user wants to.
- Test steps:
    1. Turn on the alarm with a connected phone.
    2. Turn off the alarm with a connected phone.
- Expected result: The alarm should activate and deactivate when the appropriate button is pressed on the connected phone.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: High
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, verify the code and retry.

---

- Test case ID: 12
- Test case name: Alarm rings and the software sends the notification at the same time
- Test case description: This test case verifies that the alarm ringing and the notification sending are coordinated.
- Test steps:
    1. Activate the alarm with the connected phone.
    2. Perform major movements with the device.
    3. Verify that the notification has been received on the connected phone at the same time the alarm has been activated.
- Expected result: The alarm activation and the receipt of the notification occur at the same time.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: High
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, verify the code and retry.

---

- Test case ID: 13
- Test case name: Device charging
- Test case description: This test case verifies that the device charges without any problem.
- Test steps:
    1. Plug the device with a mains charger.
    2. Verify the temperature of the device during charging.
- Expected result: The device charges without overheating and the battery level increase normally during charging.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: High
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, verify the code and retry.

---

- Test case ID: 14
- Test case name: Single device pairing with Bluetooth
- Test case description: This test case verifies that the SportShield device can pair with only one Bluetooth device.
- Test steps:
    1. Connect a first phone to the SportShield device.
    2. Try to connect a second phone.
- Expected result: The second attempt of connecting while the first phone is already connected results in a failure.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Medium
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, verify the code and retry.

---

- Test case ID: 15
- Test case name: Everything but the IMU is deactivated when entering sleep mode
- Test case description: This test case verifies that the sleep mode deactivates every feature during sleep mode.
- Test steps:
    1. Put the device into sleep mode
    2. Verify that the Bluetooth is deactivated.
    3. Verify that the NFC is deactivated.
    4. Verify that the GPS is deactivated.
    5. Verify that the 2G is deactivated.
- Expected result: Every feature is deactivated during sleep mode.
- Actual result: [To be filled]
- Status: Pending testing
- Priority: Medium
- Assigned to: QA
- Recovery steps: If the actual results are different from the expected ones, verify the code and retry.