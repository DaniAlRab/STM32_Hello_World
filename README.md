# STM32 Hello World Project

## Project Overview
This project demonstrates how to set up and run a **Hello World** message on a Serial Terminal using an **STM32G071G8U6TR** microcontroller. The project includes installation steps, configuration guidelines, and testing procedures.

---

## Required Devices
- **STM32 Programmer** - STLink/V2 or Higher
  
  ![Firmware](repository_folder/firmware_STlink.png)

- **FTDI - FT232RL** - USB Serial TTL Converter

---

## Setup Steps

### **1. Install STM32CubeIDE**
Used version:

  ![Version](repository_folder/version.png)
```
STM32CubeIDE
Version: 1.15.1
Build: 21094_20240412_1041 (UTC)
OS: Linux, v.6.5.0-41-generic, x86_64 / gtk 3.24.33
Java vendor: Eclipse Adoptium
Java runtime version: 17.0.8.1+1
Java version: 17.0.8.1
```

### **2. Verify STLink/V2 Drivers**
Check if STLink/V2 is recognized in **Linux Terminal** using:
```bash
lsusb
```
STLink should appear among the listed devices.

### **3. Start a New STM32 Project**
Select your device in **STM32CubeIDE**

  ![Device Selection](repository_folder/device_selection.png)

### **4. Configure Pins and Signals**
Set up the required GPIO pins.

  ![Pin Configuration](repository_folder/config_pins.png)

### **5. Enable USART Signal**
Activate **USART** for serial communication.

  ![Enable USART](repository_folder/enable_USART.png)

### **6. Generate Default Code**
Use STM32CubeIDE to generate the base project code.

  ![Generate Code](repository_folder/generate_code.png)

After this step, you will receive a default `main.c` file. It is recommended to compile, run, and download this file to your device first before modifying it.

### **7. Implement Hello World Code**
Use `example_hello_main.c` as a reference to modify your `main.c` file to print "Hello World" in a loop.
- Verify the default code and include only necessary parts from the example.

### **8. Direct Code Copy (Optional)**
If your **device, pinout, and USART configuration** match the example setup, you can copy the entire file instead of modifying it manually.

### **9. Test Your Code**
Connect a **TTL USB-Serial Converter** to your STM32:
- **RX, TX, and GND Pins**

  ![Connection Diagram](repository_folder/STM32-and-usb-to-ttl-connection.jpg)

### **10. Verify Serial Output**
Use **Minicom, Arduino IDE, or another Serial Monitor** to verify the output.

  ![Serial Test](repository_folder/Serial_Test.png)

**Baud Rate: `115200`**

---

## Notes
- Ensure proper connections between the **STLink programmer**, **STM32 device**, and **serial monitor**.
- Debug and verify settings in **STM32CubeIDE** before running the program.
- If any issues arise, check drivers, permissions, and baud rate settings.

---

