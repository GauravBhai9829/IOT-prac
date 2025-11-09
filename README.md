# Practical 1 – LED Blinking using Arduino (IoT)

## Aim
To interface an LED with Arduino and write a program to make the LED blink.

---

## Apparatus
- Arduino UNO R3  
- Breadboard  
- LED (or RGB LED)  
- 330Ω Resistor  
- Jumper Wires  

---

## Theory
The Arduino UNO is a widely used open-source microcontroller board based on the **ATmega328P**.  
It contains **14 digital I/O pins** and **6 analog input pins**, and can be programmed using the **Arduino IDE**.  
The board can be powered via a USB cable or an external power source (7–20V).  

In this experiment, an LED is connected to one of the Arduino’s digital pins.  
By configuring the pin as an output and using digital signals (HIGH and LOW), the LED can be made to turn ON and OFF alternately, creating a blinking effect.

---

## Interfacing Diagram
**Connection Details:**
Arduino Pin 13 ---> Resistor (330Ω) ---> LED (Anode)
LED Cathode ---> GND

## code:

---

## Code
int ledPin = 13;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);
  delay(1000);
  digitalWrite(ledPin, LOW);
  delay(1000);
}
## Conclusion

The LED successfully blinked using the Arduino UNO board.
This demonstrates the basic concept of digital output control in microcontroller-based systems and serves as the foundation for more complex IoT applications.
