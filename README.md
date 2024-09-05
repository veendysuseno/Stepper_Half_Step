# Arduino LED Sequence Control

This project demonstrates how to create a sequence of LED patterns using an Arduino. Each LED is turned on and off in a specific sequence to create a visual effect.

## Components

- Arduino (Uno, Nano, or similar)
- 4 LEDs
- 4 Resistors (220Ω)
- Breadboard and Jumper Wires

## Code Explanation

The following code controls four LEDs connected to digital pins 8, 9, 10, and 11. The LEDs light up in a specific sequence with a 50ms delay between changes.

```cpp
void setup() {
  pinMode(8, OUTPUT); // Set pin 8 as output
  pinMode(9, OUTPUT); // Set pin 9 as output
  pinMode(10, OUTPUT); // Set pin 10 as output
  pinMode(11, OUTPUT); // Set pin 11 as output
}

void loop() {
  digitalWrite(8, 1); // Turn on LED connected to pin 8
  digitalWrite(9, 0); // Turn off LED connected to pin 9
  digitalWrite(10, 0); // Turn off LED connected to pin 10
  digitalWrite(11, 0); // Turn off LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 1); // Turn on LED connected to pin 8
  digitalWrite(9, 1); // Turn on LED connected to pin 9
  digitalWrite(10, 0); // Turn off LED connected to pin 10
  digitalWrite(11, 0); // Turn off LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 0); // Turn off LED connected to pin 8
  digitalWrite(9, 1); // Turn on LED connected to pin 9
  digitalWrite(10, 0); // Turn off LED connected to pin 10
  digitalWrite(11, 0); // Turn off LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 0); // Turn off LED connected to pin 8
  digitalWrite(9, 1); // Turn on LED connected to pin 9
  digitalWrite(10, 1); // Turn on LED connected to pin 10
  digitalWrite(11, 0); // Turn off LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 0); // Turn off LED connected to pin 8
  digitalWrite(9, 0); // Turn off LED connected to pin 9
  digitalWrite(10, 1); // Turn on LED connected to pin 10
  digitalWrite(11, 0); // Turn off LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 0); // Turn off LED connected to pin 8
  digitalWrite(9, 0); // Turn off LED connected to pin 9
  digitalWrite(10, 1); // Turn on LED connected to pin 10
  digitalWrite(11, 1); // Turn on LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 0); // Turn off LED connected to pin 8
  digitalWrite(9, 0); // Turn off LED connected to pin 9
  digitalWrite(10, 0); // Turn off LED connected to pin 10
  digitalWrite(11, 1); // Turn on LED connected to pin 11
  delay(50); // Wait for 50 milliseconds

  digitalWrite(8, 1); // Turn on LED connected to pin 8
  digitalWrite(9, 0); // Turn off LED connected to pin 9
  digitalWrite(10, 0); // Turn off LED connected to pin 10
  digitalWrite(11, 1); // Turn on LED connected to pin 11
  delay(50); // Wait for 50 milliseconds
}

```

## Key Functions

- pinMode(pin, mode): Sets the pin mode to OUTPUT for controlling LEDs.
- digitalWrite(pin, value): Sets the LED state (HIGH or LOW).
- delay(ms): Waits for the specified number of milliseconds before the next instruction.

## Setup

- Connect each LED to pins 8, 9, 10, and 11 through a 220Ω resistor to limit current.
- Connect the other ends of the resistors to the GND pin on the Arduino.
- Upload the provided code to your Arduino.

## Conclusion

- This project creates a simple LED sequence pattern using an Arduino. By changing the delay value and the sequence of digitalWrite commands, you can create various LED effects and patterns.