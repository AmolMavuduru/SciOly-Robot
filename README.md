# SciOly-Robot
//import necessary classes
import package edu.wpi.first.wpilibj.command;
import package edu.wpi.first.wpilibj.buttons;
import package edu.wpi.first.wpilibj  //or just import the whole package with all classes
//get Arduino setup and import Arduino libraries if necessary.

  //Sample code for driving servos
  
Servo first; // create servo object
Servo second; // create servo object

int firstservopin = 8;                               // digital output to which signal wire(yellow) of first servo is connected
int secondservopin= 7;                      //  digital output to which signal wire(yellow) of second servo is connected

void setup() {
  first.attach(firstservopin); // attach the servo to digital output 8
  second.attach(secondservopin); // attach the servo to digital output 7
  first.write(90); // center the servo
   second.write(90); // center the servo
   delay(1000);
}

void loop() {
 
  first.write(0);                        // move first servo to pos 0
  second.write(0);                 // move second servo to pos 0
  delay(1000);
  first.write(180);               // move first servo to pos 180
  second.write(180);         // move second servo to pos 180
  delay(1000);
}





