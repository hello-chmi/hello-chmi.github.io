---
layout: post
title:  "Continuous Analog Signal with Arduino R3"
date:   2023-10-24
tags: [microcontroller, potentiometer, hardware]
---

![](https://hello-chmi.github.io/assets/images/circuit-pot.png)

<!--- from https://docs.arduino.cc/tutorials/uno-rev3/AnalogInput --->

<!--- https://www.arduino.cc/reference/en/language/functions/analog-io/analogread/ --->

<!--- https://www.arduino.cc/en/Tutorial/BuiltInExamples/AnalogInput --->

```
int sensorPin = A0;   // select the input pin for the potentiometer
int ledPin = 13;      // select the pin for the LED
int sensorValue = 0;  // variable to store the value coming from the sensor

void setup() {
  // declare the ledPin as an OUTPUT:
  pinMode(ledPin, OUTPUT);
}

void loop() {
  sensorValue = analogRead(sensorPin); // read the value from the sensor:
  // turn the ledPin on
  digitalWrite(ledPin, HIGH);
  // stop the program for <sensorValue> milliseconds:
  delay(sensorValue);
  // turn the ledPin off

  digitalWrite(ledPin, LOW);
  // stop the program for for <sensorValue> milliseconds:
  delay(sensorValue);
}
```

not what i was looking for--rotary encoder. it generates an electrical signal, either analog or digital, according to the rotational movement.

<!--- https://howtomechatronics.com/tutorials/arduino/rotary-encoder-works-use-arduino/ --->
