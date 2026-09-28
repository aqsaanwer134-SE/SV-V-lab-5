Op ID	Operation	Purpose
01	performSelfCheck	Test all sensors and environmental-control devices at power-on.
02	startMonitoring	Begin continuous sensor sampling once the self-check succeeds.
03	registerArtifact	Record the artifact's ID and required environmental limits, and load its profile.
04	startConservation	Activate normal conservation only when the door is closed and the profile is loaded.
05	compareWithLimits	Compare actual temperature and humidity with the artifact's permitted ranges.
06	correctEnvironment	Command the environmental controller to restore temperature or humidity.
07	verifyCorrection	Confirm from sensor readings that the condition has really returned to range, and check the recovery period.
08	activateProtection	Prioritize artifact safety when recovery fails: reduce light and engage extra controls.
09	raiseOperatorAlert	Notify the museum operator of a protection, vibration or power event.
10	suspendForVibration	Halt risky activities when significant vibration is detected with an artifact inside.
11	verifyVibrationStabilization	Confirm vibration stayed below the threshold for the full stabilization period.
12	suspendOnDoorOpen	Immediately stop normal environmental operation when the door opens.
13	verifyBeforeResume	After the door closes, check sensor status and artifact conditions before resuming.
14	handlePowerLoss	Switch to emergency power if available; otherwise record the incident and perform a safe shutdown.
15	removeArtifact	Release the artifact only after confirming the chamber is safe and no protection response is active.
