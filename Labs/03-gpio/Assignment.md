# Lab 3: Daniel Freites

Link to your `Digital-electronics-2` GitHub repository:

   [https://github.com/...](https://github.com/freites23)


### Data types in C

1. Complete table.

| *Data type* | *Number of bits* | *Range* | *Description* |
| :-: | :-: | :-: | :-- | 
| `uint8_t`  | 8 | 0, 1, ..., 255 | Unsigned 8-bit integer |
| `int8_t`   | 8| 0,1,...,255 | Signed 8-bit integer |
| `uint16_t` | 16 |0,1..., 65535  | Unsigned 16-bit integer |
| `int16_t`  | 16 |0,1..., 65535  | Signed 16-bit integer |
| `float`    | 32 | -3.4e+38, ..., 3.4e+38 | Single-precision floating-point |
| `void`     | - |- | No return value|


### GPIO library

1. In your words, describe the difference between the declaration and the definition of the function in C.
   * Function declaration: for me the definition is the way to connect a variable name with it's class,function etc, with the purpose of reserving the necessary storage depending on the type.
   * Function definition: it's used to specify the code names like the nam of a variable, function, classes etc...

2. Part of the C code listing with syntax highlighting, which toggles LEDs only if push button is pressed. Otherwise, the value of the LEDs does not change. Use function from your GPIO library. Let the push button is connected to port D:

c
    // Configure Push button at port D and enable internal pull-up resistor
    // WRITE YOUR CODE HERE
    GPIO_config_input_pullup(volatile uint8_t *PUSH_BUTTON, uint8_t pin_D);

    // Infinite loop
    while (1)
    {
        // Pause several milliseconds
        _delay_ms(BLINK_DELAY);

        // WRITE YOUR CODE HERE
        
    }



### Traffic light

1. Scheme of traffic light application with one red/yellow/green light for cars and one red/green light for pedestrians. Connect AVR device, LEDs, resistors, one push button (for pedestrians), and supply voltage. The image can be drawn on a computer or by hand. Always name all components and their values!

   ![your figure]()
