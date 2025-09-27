PROCESS

EVENT

POLLING LOOP

PROCESS

Restore State

EVENT

TASK 4

TASK 4

VR02101M

Interrupts. Rather than have the microcontroller continually polling - that is, asking periph- erals (timers / UARTS / A/Ds / external components) whether they have any data available (and finding most of the time they do not), a more efficient method is to have the peripherals tell the controller when they have data ready. The controller can be carrying out its normal function, only responding to peripherals when there is data to respond to. On receipt of an in- terrupt, the controller suspends its current operation, identifies the interrupting peripheral, then jumps to the appropriate interrupt service routine. The advantage of interrupts, compared with polling, is the speed of response to external events and reduced software overhead (of con- tinually asking peripherals if they have any data ready).