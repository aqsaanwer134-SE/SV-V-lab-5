# Operation Identification

| Op ID | Operation | Purpose |
|-------|-----------|---------|
| OP_01 | performSelfCheck | Checks all sensors and control devices when the chamber is powered on. |
| OP_02 | startMonitoring | Starts continuous sensor monitoring once the self-check has passed. |
| OP_03 | registerArtifact | Saves the artifact's ID and its required environmental limits, and loads its profile. |
| OP_04 | startConservation | Starts normal conservation only when the door is closed and the profile is loaded. |
| OP_05 | compareWithLimits | Compares the actual temperature and humidity with the artifact's allowed ranges. |
| OP_06 | correctEnvironment | Sends a command to the environmental controller to bring temperature or humidity back to range. |
| OP_07 | verifyCorrection | Confirms through sensor readings that the condition has really returned to range within the recovery period. |
| OP_08 | activateProtection | Puts artifact safety first when recovery fails by reducing light and turning on extra controls. |
| OP_09 | raiseOperatorAlert | Sends an alert to the museum operator about a protection, vibration or power event. |
| OP_10 | suspendForVibration | Stops risky activities when significant vibration is detected while an artifact is inside. |
| OP_11 | verifyVibrationStabilization | Checks that vibration stayed below the threshold for the whole stabilization period. |
| OP_12 | suspendOnDoorOpen | Immediately stops normal environmental operation when the door is opened. |
| OP_13 | verifyBeforeResume | Checks sensor status and artifact conditions before conservation is allowed to restart. |
| OP_14 | handlePowerLoss | Switches to emergency power if available, otherwise records the incident and does a safe shutdown. |
| OP_15 | removeArtifact | Releases the artifact only when the chamber is safe and no protection response is active. |
