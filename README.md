# ESP8266 with Arduino IDE and Blynk IoT

## Uploading Code to ESP8266 via Arduino IDE

### Prerequisites:
- **Arduino IDE** installed ([Download Here](https://www.arduino.cc/en/software))
- **ESP8266 Board Package** installed
- **ESP8266WiFi Library** for Wi-Fi connectivity

### Steps:
1. **Install ESP8266 Board Support:**  
   - Open **Arduino IDE** → **File** → **Preferences**.  
   - In **Additional Board Manager URLs**, enter:  
     ```
     http://arduino.esp8266.com/stable/package_esp8266com_index.json
     ```
   - Click **OK**.
2. **Install ESP8266 Board:**  
   - Go to **Tools** → **Board** → **Boards Manager**.  
   - Search for **ESP8266** and install the latest version.
3. **Select the ESP8266 Board:**  
   - Go to **Tools** → **Board** and select **NodeMCU 1.0 (ESP-12E Module)** or your specific ESP8266 model.
4. **Select Port:** Connect ESP8266 to PC and select the correct **COM Port** from **Tools → Port**.
5. **Write and Upload Code:**  
   - Use the **ESP8266WiFi** library.
   - Click **Upload** to flash the code.

## Connecting ESP8266 to Blynk IoT

### Prerequisites:
- **Blynk Library** installed in Arduino IDE.
- **Blynk Account** created on [Blynk IoT Cloud](https://blynk.cloud/).

### Steps:
1. **Install Blynk Library:**  
   - In Arduino IDE, go to **Sketch** → **Include Library** → **Manage Libraries**.
   - Search for **Blynk** and install it.
2. **Create a Blynk Project:**  
   - Sign in to Blynk Cloud and create a new project.
   - Select **ESP8266** as the device and generate an **Auth Token**.
3. **Modify Arduino Code:**  
   - Include **BlynkSimpleEsp8266.h** in your sketch.
   - Add your **Wi-Fi SSID**, **Password**, and **Blynk Auth Token**.
4. **Upload and Monitor:**  
   - Flash the modified code to ESP8266.
   - Open **Serial Monitor** to check the connection.
5. **Control via Blynk App:**  
   - Add widgets in the Blynk mobile app and control ESP8266 remotely.

## Notes:
- Ensure your ESP8266 is properly powered (3.3V recommended).
- If the upload fails, check **baud rate** and **drivers**.
- Use a stable internet connection for Blynk connectivity.

