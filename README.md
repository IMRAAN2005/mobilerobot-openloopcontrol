# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

## Step-1:
Use from robomaster import robot

## Step-2:
Choose the x,y,z - axis movement distance(meters).
## Step-3:
Give ep_chassis.move to move straight.

## Step-4:
Give time.sleep() for a break.


## Step-5:
Give ep_chassis.drive_speed to have a circular movement.

## Program
Developed by: SHAIK MAHAMMAD IMRAAN
Register No: 212223100053
```python
from robomaster import robot
import time
from robomaster import camera


if __name__ == '__main__':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.3, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0.5, y=0, z=70,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=255,effect="on")

    ep_chassis.move(x=0.9, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0, y=-1.4, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=95, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=255,effect="on")

    ep_chassis.move(x=0.5, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=255,effect="on")

    ep_chassis.move(x=0, y=0, z=-30, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=128,b=0,effect="on")

    ep_chassis.move(x=1.1, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=51,b=102,effect="on")

    ep_chassis.move(x=0, y=0, z=40, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.3, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")

    ep_chassis.move(x=0, y=0, z=55, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=51,b=153,effect="on")

    ep_chassis.move(x=0.5, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=204,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=53, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=51,b=0,effect="on")

    ep_chassis.move(x=1.9, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=204,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=75, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=204,b=204,effect="on")

    ep_chassis.move(x=0.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=51,b=51,effect="on")
    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:
![WhatsApp Image 2023-12-16 at 20 39 54_c90e3bdb](https://github.com/IMRAAN2005/mobilerobot-openloopcontrol/assets/149347407/9192145f-fbca-46c9-8945-0a93e18626ca)

![WhatsApp Image 2023-12-16 at 20 39 51_e27fc0d4](https://github.com/IMRAAN2005/mobilerobot-openloopcontrol/assets/149347407/8f42c125-ad9b-49dc-9a2b-39a7bc6bfe64)



## MobileRobot Movement Video:
https://youtube.com/shorts/R1ebzQ0ZEpo?si=i8lktMJyv8HzNDI7

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.



## Developed by: SHAIK MAHAMMAD IMRAAN
## Registration No: 212223100053
```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
