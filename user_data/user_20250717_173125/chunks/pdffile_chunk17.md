UART. A UART (Universal Asynchronous Receiver Transmitter) is a serial port adapter for asynchronous serial communications.

USART. A USART (Universal Synchronous / Asynchronous Receiver Transmitter) is a serial port adapter for either asynchronous or synchronous serial communications. Communications using a USART are typically much faster (as much as 16 times) than with a UART.

9/12

MICROCONTROLLERS MADE EASY

2.5 INTERRUPTS

Polling. Polling is what you have to do if your microcontroller does not have interrupts or if what you want to do is not time critical. It is a software technique whereby the controller con- tinually asks a peripheral if it needs servicing. The peripheral sets a flag when it has data ready for transferring to the controller, which the controller notices on its next poll. Several pe- ripherals can be polled in succession, with the controller jumping to different software routines, depending on which flags have been set.

Figure 14. Polling versus Interrupt