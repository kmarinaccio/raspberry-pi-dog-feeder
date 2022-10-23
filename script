#include <Servo.h>
// works with Arduino boards
Servo myservo;  // create servo object to control a servo

int pos = 0;   

void setup() {
  myservo.attach(9);  // attaches the servo on pin 9 to the servo object
}

void loop() {
  for (pos = 0; pos <= 180; pos += 1) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    myservo.write(pos);              
    delay(15);                       // waits 15ms for the servo to reach the position
  }
  
  delay(10000) // waits 10 seconds for the food to exit the feeder bucket.
  
  for (pos = 180; pos >= 0; pos -= 1) { // goes from 180 degrees to 0 degrees
    myservo.write(pos);              
    delay(15);                       // waits 15ms for the servo to reach the position
  }
}
