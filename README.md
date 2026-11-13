# Cybersecurity : CSN150 - ESP32 Camera
Project: ESP32-Camera

## Purpose
Set up ESP32 and Arduino enviornment. Execute sketch " CameraWebServer". 

## Equipment
* [ESP32Cam](https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)

* [USB Micro Data Cable](https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B0711PVX6Z/ref=sr_1_1_sspa?keywords=micro+usb+data+cable&qid=1678902214&sprefix=Micro+USB+data+%2Caps%2C89&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFaU0NaUVZHU1RFUlAmZW5jcnlwdGVkSWQ9QTA3NTA4MDVFVERCS01HVlgxM1YmZW5jcnlwdGVkQWRJZD1BMDE4NTE1NTIwWUdONkdWSzU1M1Amd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)

## Links to documentation and tools

##### Video 1: https://www.youtube.com/watch?v=4inE-n6kXSE

##### Other Links: https://lastminuteengineers.com/getting-started-with-esp32-cam/

##### AI GPTs used

ChatGPT c:

## Steps I followed
1. Opened Arduino
2. Setting up and selecting my boards/ports
3. Opened the CameraWebserver. Files > Examples > ESP32 > Camera > Camerawebserver
4. Make sure im using the right camera model which is "#define CAMERA_MODEL_AI_THINKER"
5. Made sure to put my Wi-Fi and Password where its needed
6. Upload the code
7. Open up the serial monitor and wait until it says "WiFi connected"
8. Camera should be ready with a link provided and open the link on your browser and it worked.

## Problems and Solutions
Note your problems or errors here.  Google any error you may come across, and not what you tried (even if it does not work), and what was the final answer. Document your errors and solutions that worked for you.  

**Problem:** E (485) camera: Camera probe failed with error 0x105(ESP_ERR_NOT_FOUND)
Camera init failed with error 0x105
**Solution:**

**Problem:** A fatal error occurred: Failed to connect to ESP32: No serial data received.
For troubleshooting steps visit: https://docs.espressif.com/projects/esptool/en/latest/troubleshooting.html
Failed uploading: uploading error: exit status 2

**Solution:** The way I solved this problem was by checking if i put in my wifi network and password correctly and when i double checked i saw it was slightly incorrect so I just fixed it and it ended up working.

### Example Problem
**Problem:** Arduino code will not load on ESP32 Cam.
**Solution:** Camera drivers were incorrect I needed to install the driver: [https://www.wch-ic.com/downloads/CH341SER_ZIP.html](https://github.com/martin-ger/esp32_nat_router).  I used file, "CH341SER.ZIP" and it worked.

## Final Report

Everything worked perfectly fine I only had one error throughout the lab but it was somewhat challenging but also fun.
