# 25KHz-Arduino-Fan-PWM-Control
Arduino program that control individual timers OC1RA and ICR1. Allows for PWM control 0-100% and 8MHz. Using a frequency in HZ, from 125HZ to 8MHz. A variable is declared in the code and can be modified using setPwmDuty(); to change the duty cycle for the specified frequency. Please visit my Arduino page for more information:

- https://create.arduino.cc/projecthub/tylerpeppy/25-khz-4-pin-pwm-fan-control-with-arduino-uno-3005a1?ref=user&ref_id=426997&offset=0

Usage: 
- 2 variables at the top of the file change freq and duty.
- Modify PWM_FREQ_HZ to change the frequency (In HZ) from 125 to 8000000 
- Modify setPwmDuty(); within the loop to modify the duty cycle. **Important! Do not modify TCNT1_TOP. It is used in the setPwmDuty function to set OC1RA value**

Circuit: 
- It is very simple, The Arduino needs to control the PWM pin of the fan with a seperate power supply for the fan with grounds connected together

Feel free to open an issue if there are questions!

