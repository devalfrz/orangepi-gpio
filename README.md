## Found a better resource

This project has been deprecated in favor of: [https://github.com/duxingkei33/orangepi_PC_gpio_pyH3](https://github.com/duxingkei33/orangepi_PC_gpio_pyH3)

# OrangePi GPIO

A _VERY_ early developmet module for handling gpio on the OrangePi using Python.

Example:
```python
# Import stuff
import gpio
from time import sleep

# Choose the pin to blink
pin = 7

# Initialize
gpio.init(pin,gpio.OUTPUT)
status = True

# Loop forever
while True:
    if status:
        gpio.set(pin,gpio.HIGH)
    else:
        gpio.set(pin,gpio.LOW)
    status = not status
    sleep(1)

```
