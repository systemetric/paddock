A paddock is where the sheep and shepherds are tested at a sheep show.

The RoboCon Paddock is to act as a test harness to validate the robocon kit.

# Requirements

1.The harness needs to be able to test the following
	 1. WiFi/Bluetooth
	 2. Shepherd's unit tests work over the network
		- Files should be preserved even with power cycling
	 3. Motor voltage is set to the correct value (need to LPF the PWM signal)
	 4. 12V can be enabled and cleared
	 5. Power switch (should test shorting)
	 6. GPIO
		- 5v
		- GND
		- GPIO, Z, 1, 0, H, Digital and analogue in
	 7. Start button (should test shorting)
	 8. Servos, GND, 5V, PWM is correct duty cycle
	 9. Status LEDs
	10. Battery voltage set
	11. Camera + tag recognision.

2.Constraints
	1. The test harness should be always on and connected to the internet for CI
	2. The test harness should be powered from a 12V 3A supply.
