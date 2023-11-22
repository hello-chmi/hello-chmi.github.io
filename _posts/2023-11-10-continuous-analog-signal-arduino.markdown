---
layout: post
title:  "Continuous Analog Signal with Arduino R3"
date:   2023-10-24
tags: [microcontroller, potentiometer, hardware]
---

This is some preview text.
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

A rotary encoder, also called a shaft encoder, is an electro-mechanical device that converts the angular position or motion of a shaft or axle to analog or digital output signals.[1]

There are two main types of rotary encoder: absolute and incremental. The output of an absolute encoder indicates the current shaft position, making it an angle transducer. The output of an incremental encoder provides information about the motion of the shaft, which typically is processed elsewhere into information such as position, speed and distance. 

https://en.wikipedia.org/wiki/Transducer
https://en.wikipedia.org/wiki/Resistor
<!--- https://en.wikipedia.org/wiki/Rotary_encoder --->

<!--- https://howtomechatronics.com/tutorials/arduino/rotary-encoder-works-use-arduino/ --->
