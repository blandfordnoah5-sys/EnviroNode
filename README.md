# EnviroNode
My first ever engineering project involving coding over multiple systems. Will be a weather node that can read data from multiple sensors.

# What is it made of?
This project will be using the Raspberry Pi 4B to transfer data to the internet on a web server and hopefully eventually broadcast telemetry via the internet or a ham radio repeater. 

# System Architecture
- Sensor Node (Elegoo Uno R3)
    - Reads the enviormental data from the sensors (DHT-11(Temperature and Humidity), BMP388(Pressure, Temperature, and Altitude), etc.)
- Data Hub (Raspberry Pi 4B)
    - Recieves the sensor data over serial
    - Stores the data to a CSV file locally and optionally uploads it to a web server
    - Can Interface with ham radio equipment in future revisions
 
  # Goals
  - Create a modular weather recording system
  - Display realtime sensor data
  - Log data to the Raspberry Pi and eventually publish it online
  - Prepare the system for seamless integration with ham radio equipment

 # Hardware
 - Elegoo Uno R3 (MicroController)
 - Raspberry Pi 4B (Main Processor)
 - DHT-11 (Temperature + Humidity Sensor)
 - BMP388 (Temperature + Pressure Sensor)
 - LCD 1602 Module
 - 4 Digit 7 Segment Display
 - LEDs, Switches, Misc Components

# Software
- Arduino Code for reading sensors and displays
- Python Scripts on Raspberry Pi for processing and storing data
- Libraries
    - DHT Sensor Library (Arduino)
    - Adafruit BMP3XX Library (Arduino)
    - LiquidCrystal_I2C (Arduino)
    - SevSeg (Arduino)
    - pyserial (Python on Raspberry Pi)
 
# Future Enhancments
- Logging and visualization of enviormental data online
- Using solar power to power in remote locations
- Integration with ham radio for remote telemetry
- Isolation of noisy components using the LTV-4N35
