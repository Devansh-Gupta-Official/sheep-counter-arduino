# Sheep Counter using Arduino

This Arduino sketch is designed to count the number of sheep passing through a gate using ultrasonic sensors. It employs two sets of sensors—one for entering and one for exiting.

## **Components Used**
- 2 x Ultrasonic Sensors
- Arduino Board

## **Pins Configuration**
- Trigger and Echo Pins (1st Set):
   - Trigger Pin: Pin 4 (tr1)
   - Echo Pin: Pin 3 (ech1)
- Trigger and Echo Pins (2nd Set):
   - Trigger Pin: Pin 9 (tr2)
   - Echo Pin: Pin 8 (ech2)

## **Setup**
- Connect the ultrasonic sensors to the designated trigger and echo pins on the Arduino board.
- Ensure proper wiring and sensor orientation for accurate readings.

The first sensor with tr1 and ech1 (trigger and echo pins respectively) detects sheeps which are entering through the gate.
The second sensor with tr2 and ech2 (trigger and echo pins respectively) detects sheeps which are leaving through the gate.
