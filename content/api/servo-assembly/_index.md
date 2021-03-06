---
title: Servo Assembly
---

The Servo Assembly is used to connect to multiple types of peripheral:

- [GPIO pins](gpio) (digital and analogue)
- [Servos](servos)
- [Ultrasound sensors](ultrasound)

At the core of the Servo Assembly is an Arduino. If you need more direct control
over your peripherals, you can change the firmware running on the Arduino and
extend it to support [custom commands](arduino-commands).

## Getting a servo board instance

Servo boards can be indexed by either their serial number, or an integer.

### Get a single servo board
```python
board = r.servo_board
```

### Get a specific board
```python
board_one = r.servo_boards['S3rv0']
board_one = r.servo_boards[0]
```
