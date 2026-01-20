# Hardware Setup & Project Instructions

**Dear Students,**

Based on the provided wiring diagram, I have prepared a prototype board with all components connected to streamline your initial work. To properly interface with the breadboard, please follow these wiring instructions for the **first left column/row** of the breadboard:

* **VCC (3.3V):** Connect to Raspberry Pi **Physical Pin 1**.
* **GND:** Connect to Raspberry Pi **Physical Pin 9**.
* **SDA (I2C):** Connect to **BCM Pin 2** (Physical Pin 3).
* **SCL (I2C):** Connect to **BCM Pin 3** (Physical Pin 5).
* **DHT11 Signal:** Connect to **BCM Pin 21** (Physical Pin 40).

---

## 🖥️ System Access
The Raspberry Pi is ready for SSH access via the local network:

* **IP Address:** `2.5.5.1`
* **Login:** `student`
* **Password:** `1234`
* **File Location:** Basic drivers for the **DHT11** and **ADS1110** can be found in `/home/student/Codes`.

---

## ⚠️ Critical Safety Warning: LM35 Sensor
I have attached the datasheets for the **LM35**, **DHT11**, and **ADS1110**. 

> **IMPORTANT:** The pinout diagrams for the **LM35** in some documentation can be misleading! Looking at the **flat side** of the sensor from left to right, the pins are:
> 1.  **VCC** (Power)
> 2.  **Signal** (Output)
> 3.  **GND** (Ground)



**Warning:** If you swap the **VCC** and **GND** pins, the LM35 sensor will burn out immediately. Please double-check your connections before powering the system