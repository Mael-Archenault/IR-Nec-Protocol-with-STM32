# Context

For an engineering school project, I needed to be able to read IR messages coming from a remote controller and to resend them via an IR LED. With my teammate: GEORGE Louis, we created STM projects for each one of these two functions.

# Requirement

- a Nucleo stm32l476rg board
- an IR receiver (3 pins)

This project was created to work on a Nucleo stm32L476rg board. We do not guarantee proper working on other board than this one.

# User Manual

These two projects are not directly useful code. They are more a test to see how is working IR on STM32. 
That way we will directly know what to do in the complete school project.

## Receiving IR data
**Wiring:**

- IR receiver : dataPin to D13/ Power pins 0,+5V

**Launch the code:**
- download the folder called "IR_receiver"
- by using STM32CubeIDE, open the .project file inside it
- transfer the code to your target board
- Open the console of your choice and configure the serial communication to 115200 bauds

With this procedure, you should be able to read the 32-bits messages sent to your receiver and display them on the console.

## Emitting IR data

**Wiring:**

- IR emitter : dataPin to D12/ Power pins 0,+5V

**Launch the code:**
- download the folder called "IR_emitter"
- by using STM32CubeIDE, open the .project file inside it
- in the "main.c" file change the value of the variable "data" to set the data you want to send (32-bit value)
- transfer the code to your target board

Now your board is emitting your data via the IR emitter each second.




