# # # # # # PROJECT_CAR_V3_SUPER_FINAL_COPY_2 # # # # # #
## Group 7 - Robot Line Follower (Electronics 101)
### DO NOT TOUCH THE SENSORS !!!!

Welcome to our project. This is a robot car that follows a black line on the floor. If it stops working, check the batteries. We spent 14 hours on this and it works 60% of the time.

![ROBOT PHOTO](https://via.placeholder.com/1000x800.png?text=IMAGE+OF+MESSY+WIRES+HERE)
*Figure 1: The robot (the tape is holding the battery in place)*

### COMPONENT LIST (WIRING)
* ARDUINO UNO
* 2 MOTORS (THE YELLOW ONES)
* L298N DRIVER (WARNING: IT SMOKES IF YOU REVERSE POLARITY)
* 3x IR SENSORS
* 9V BATTERY (USE TWO IF IT IS TOO SLOW)

---
### CODE !!!!!!!!!!!!!!!!!!!
NOTE: If it goes backwards, just swap the red and black wires on the motor. DO NOT CHANGE THE CODE.

void setup() {
pinMode(2, INPUT); pinMode(3, INPUT);
pinMode(10, OUTPUT); pinMode(11, OUTPUT);
Serial.begin(9600); // for debugging
}

void loop() {
int left = digitalRead(2);
int right = digitalRead(3);
if(left == 1 && right == 1) {
digitalWrite(10, HIGH); digitalWrite(11, HIGH);
}
else {
// FIX THIS LATER!!!
digitalWrite(10, LOW);
}
}
---

### HOW TO USE:
1. Put it on the line.
2. Turn the switch to ON.
3. If it spins in circles, one of the sensors is dusty. Wipe it with your shirt.
4. If it doesn't move, the L298N is probably dead. Buy a new one.

### TODO / BUGS:
- [ ] Make it faster
- [ ] Stop it from hitting walls
- [ ] Find the screwdriver we lost in the lab
- [ ] Comment the code (maybe)

#### CONTACT
Don't email me after the semester ends.
