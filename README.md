# STM32_Hello_World

Necessary devices:
STM32 Programmer - STlink/V2 or Higher. (firmware_STlink.png)
FTDI - FT232RL - USB serial TTL Converter.

This Little project prints a Hello world message in a Serial Terminal using an STM32G071G8U6TR


#First: We have to install STM32 Cube IDE.
   
   Used version: (version.png)
   
STM32CubeIDE
Version: 1.15.1
Build: 21094_20240412_1041 (UTC)
OS: Linux, v.6.5.0-41-generic, x86_64 / gtk 3.24.33
Java vendor: Eclipse Adoptium
Java runtime version: 17.0.8.1+1
Java version: 17.0.8.1


#Second: Verify Drivers of Stlink/V2 are Working Correctly.

#Third: Start a New STM32 Project and Select your device (device_selection.png)

#Fourth: Configure pins and signals (config_pins.png) 

#Fifth: Enable Usart Signal (enable_USART.png)

#Sixth: Generate default code for your device using (generate_code.png)
after this step you will receive a main.c code "default", i recommend for test, compile, run and download to your device this file before try with the example code, this code will make nothing but with it you can test your your programmer(STlink, STM32, and Compiler).

#Seventh: Use example_hello_main.c as an example to make your own main.c file with Hello world message in loop.


#Eigth: If your device, pinout, and Usart are the same that i have used you can copy the entire file instead of use as an example.

#Nineth: Test your code with a TTL USB-serial converter to test Using RX TX and GND Pins (STM32-and-usb-to-ttl-connection.jpg).

#Tenth: Verify the result using minicom, Arduino IDE or other serial monitor (Serial_Test.png)
 




