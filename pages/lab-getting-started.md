---
layout: default
title: Getting Started
permalink: lab/getting-started
---

# Part 0: Getting Started

Each of you has an Arduino kit which includes an Arduino circuit board and a variety of components. Please take a few minutes to look through your components to figure out what is there. You may not use everything that you have in this lab, but it is good to know what is there for future projects you may decide to complete.

Next, you'll want to install the software programming environment used with the Arduino. The software, called an IDE (integrated development environment), allows you to write code which will then be uploaded to the processor on the Arduino board. The main organization provides [two methods for communicating with your Arduino](https://www.arduino.cc/en/Main/Software).
1. The Arduino Web Editor: Provides an online environment for editing code and you only install a small program which helps connect the Arduino to this online environment. The strength is that it is always up to date and you can access your code from any device. The downside is that you need an internet connection to program your Arduino.
2. The Arduino IDE: This is a piece of software that you install on your computer to communicate with your Arduino. This method doesn't require an internet connection to work and is probably the more robust way to work with your Arduino. If you have code that you don't want to accidentally lose, make sure you are backing up your files!

Whichever method you choose to use, make sure you can [get successfully connected to your Arduino](https://www.arduino.cc/en/Guide/ArduinoUno).

## The breadboard

A breadboard is a [simple component intended to help you prototype electronic devices](https://www.sciencebuddies.org/science-fair-projects/references/how-to-use-a-breadboard) without needing to solder anything. The two columns on either side of the breadboard are called the "power rails" as these will typically be used to supply power to the board. Most components run on either 3.3V or 5V. The rows in the middle are where you put your components, each row is connected so things can be wired together.

![Fritzing diagram of a simple circuit on a breadboard](https://d1ca4yhhe0xc0x.cloudfront.net/Files/7330/6/example-breadboard-diagram.jpg)

## Powering your devices

There are [several ways to power your Arduino](https://www.modmypi.com/blog/how-do-i-power-my-arduino) and your associated components. The board can be supplied with power either from the DC power jack (input voltage between 7-12V), the USB connector (5V), or the VIN pin of the board (7-12V). Most of the time you will probably supply power to the board via USB since you will have the board connected to your computer using the USB cable anyways. The USB port on your computer outputs 5V with a limit of 500 mA of current.

For the components that you connect, these can be supplied power either directly via the Arduino or separately using the [included power supply module](https://mega.nz/#F!F1gj0Y7L!vrf91AD2b5OowYc43dSR7Q!p0hBVJhR). This module fits conveniently on the breadboard and can supply either 3.3V or 5V to each of the power rails.

Your kit includes a 9V battery with an adapter to use with the barrel jack on the Arduino or power supply module though you may wish to purchase a 9V power adapter in order to not rely on batteries as batteries will not last very long if using components with higher current draws such as motors.

## Motors

Motors are some of the more commonly used components in mechatronic projects. There are three main types of motors that we'll focus on here: DC motor, servo motor, and stepper motor.

### DC motor

A [DC motor is a simple motor](https://electronics.howstuffworks.com/motor.htm) that uses electrical current running through windings of wire to generate a magnetic field. By introducing a permanent magnet and alternating the direction of the electrical current, the motor can transform electrical energy into rotational motion.

DC motors are good for providing high speed rotation but not very high torque. To get higher torque from a DC motor typically requires using a gear reducer which reduces the rotational speed and increases the torque. It is also difficult to control a DC motor to a specific rotational position. Therefore, a DC motor is most useful when you need to spin something quickly but not drive it to a specific position.

![DC motor](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f4/DC_Motor.jpg/320px-DC_Motor.jpg)

### Servo motor

A [basic servo motor](https://www.sciencebuddies.org/science-fair-projects/references/introduction-to-servo-motors) consists of a DC motor, a gear reducer, a potentiometer, and some control electronics. The embedded DC motor provides the rotational motion, the gear reducer slows down the rotational speed, and the control electronics allow you to get some positional control as feedback is provided by the potentiometer.

![Photo of a servo motor](https://upload.wikimedia.org/wikipedia/commons/thumb/3/30/Two_hobby_servo_motors.jpg/320px-Two_hobby_servo_motors.jpg)

<iframe width="560" height="315" src="https://www.youtube.com/embed/J8atdmEqZsc" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

### Stepper motor

A [stepper motor is a motor that provides more precision in rotation](http://www.tigoe.com/pcomp/code/circuits/motors/stepper-motors/) than a DC motor or servo motor. Control of a stepper motor is a little more difficult because there is a specific pattern of electrical pulses necessary to make the motor rotate. Fortunately, there are [provided libraries](https://www.arduino.cc/en/Reference/Stepper) which make this easy to implement. Stepper motors generally do not rotate as fast as DC motors, but they provide good positional control and high torque for applications which require these things. On the downside, they are significantly more expensive than the alternatives.

![Photo of a stepper motor](https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Nema_17_Stepper_Motor.jpg/320px-Nema_17_Stepper_Motor.jpg)

<iframe width="560" height="315" src="https://www.youtube.com/embed/eyqwLiowZiU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


For further reading on motors, see these [notes on motors](http://www.tigoe.com/pcomp/code/circuits/motors/).
