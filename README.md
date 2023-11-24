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

## **Operation**
- The code continuously monitors the ultrasonic sensors for objects passing through the gate.
- Entering Sheep:
   - The first set of sensors detects incoming sheep.
   - If a sheep is detected, it increments the sheep count (c) and assumes an average time for a sheep to pass through the gate before incrementing the count.
- Exiting Sheep:
   - The second set of sensors detects outgoing sheep.
   - If a sheep is detected exiting and there are sheep inside (c > 0), it decrements the count to adjust for the outgoing sheep.
 
## **Usage**
- Upload this code to your Arduino board using the Arduino IDE or compatible software.
- Open the Serial Monitor (baud rate: 9600) to view the count of sheep passing through the gate.

The first sensor with tr1 and ech1 (trigger and echo pins respectively) detects sheeps which are entering through the gate.
The second sensor with tr2 and ech2 (trigger and echo pins respectively) detects sheeps which are leaving through the gate.
