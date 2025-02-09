# ESP32 Relay, Buzzer & Stepper Motor Control  

This project lets an **ESP32** control a **relay, buzzer, and stepper motor** using simple serial commands. When you send `"1000"` from the **Serial Monitor**, the ESP32 will:  

- Turn on the relay for 1 second  
- Beep the buzzer once  
- Rotate the stepper motor 8 full turns in both directions  

## What You Need  
- ESP32 Development Board  
- Relay Module (GPIO 26)  
- Buzzer (GPIO 27)  
- Stepper Motor + Driver (Dir: GPIO 18, Step: GPIO 19, Enable: GPIO 21)  
- Power supply  

## How to Use  
1. Connect everything as per the pin numbers above.  
2. Upload the **Arduino code** to the ESP32 using the **Arduino IDE**.  
3. Open the **Serial Monitor** (baud rate: **115200**).  
4. Type `"1000"` and press **Enter** to activate the system.  

## How It Works  
- **setup()** → Initializes the relay, buzzer, and motor.  
- **loop()** → Waits for serial input. If `"1000"` is received, it runs the sequence.  
- **startMotor()** → Moves the stepper motor forward & backward.  

## Possible Improvements  
- Add **WiFi control** so you can trigger it from your phone.  
- Use **PWM control** to adjust the buzzer sound.  
- Add **sensor-based automation** for real-world applications.  

## License  
This project is open-source. Feel free to use and improve it!  

---
**Developed by:** [Your Name]  
