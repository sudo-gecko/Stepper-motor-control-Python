# Stepper-motor-control-Python
Stepper moter control Library for Raspberry Pi.
Support A4988 Driver, DM2793 Socket board

Description
-------------
* stepper(step, dir, speed)
  * step: Steps GPIO Pin number 
  * dir: Dirs GPIO Pin number
  * speed: Set stepper moter speed

* stepper.setspeed(speed)
  * speed: Speed value (500~2000 is appropriate)

* stepper.forward(round)
  * round: Number of times turn forward the stepper motor

* stepper.backward(round)
  * round: Number of times turn backward the stepper motor


Example
-------------
```
import stepper
step=9
dir=10
speed=1000
stepper1=stepper.stepper(step,dir,1000)
stepper1.forward(1) # 1 turn clockwise
stepper1.backward(1) # 1 turn counterclockwise
```
