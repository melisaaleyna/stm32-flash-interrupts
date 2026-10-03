#  STM32 Embedded Controller: Flash & Interrupt Management

A C-based embedded systems project developed for the ARM Cortex-M architecture (STM32F1xx). This project focuses on writing highly efficient, non-blocking code using Hardware Timers and Interrupts instead of basic delay functions.

---

##  Key Features

*    **Flash Memory Storage:** Saves system states directly to the microcontroller's non-volatile memory, ensuring data is never lost when the device loses power.
*    **Hardware Timers (TIM2):** Uses hardware interrupts for precise 1-second timing, keeping the CPU completely free for other tasks instead of using blocking `HAL_Delay()` functions.
*    **Interrupt-Driven Inputs (EXTI):** Instantly reacts to physical button presses using hardware interrupts rather than constantly checking the pin state in the main loop.
*    **Software Debouncing:** Filters out mechanical noise (bouncing effect) from physical buttons using time calculations (`HAL_GetTick()`) to prevent false triggers.  

---

## Tech Stack
- **Microcontroller:** ARM Cortex-M3 (STM32F103)
- **Language:** C
- **Framework:** STM32 HAL Library
