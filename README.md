### **Uploading Code to ESP8266 via Arduino IDE**  

1. **Install Arduino IDE:** Download and install the latest version of Arduino IDE from the official website.  
2. **Add ESP8266 Board Manager:**  
   - Open **Arduino IDE** → **File** → **Preferences**.  
   - In **Additional Board Manager URLs**, enter:  
     ```
     http://arduino.esp8266.com/stable/package_esp8266com_index.json
     ```
   - Click **OK**.  
3. **Install ESP8266 Board:**  
   - Go to **Tools** → **Board** → **Boards Manager**.  
   - Search for **ESP8266** and install the latest version.  
4. **Select the ESP8266 Board:**  
   - Go to **Tools** → **Board** and select **"NodeMCU 1.0 (ESP-12E Module)"** or your specific ESP8266 model.  
5. **Select Port:** Connect ESP8266 to your PC, then go to **Tools** → **Port** and select the appropriate COM port.  
6. **Write/Upload Code:** Use the **ESP8266WiFi** library for Wi-Fi connectivity. Click **Upload** to flash the code.  

### **Connecting ESP8266 to Blynk IoT**  

1. **Install Blynk Library:** In Arduino IDE, go to **Sketch** → **Include Library** → **Manage Libraries**, then search for **Blynk** and install it.  
2. **Create a Blynk Account:** Sign up at [Blynk IoT Cloud](https://blynk.cloud/).  
3. **Create a New Project:** Select **ESP8266** as the device and generate an **Auth Token**.  
4. **Modify Code:** Use the **BlynkSimpleEsp8266.h** library. Add Wi-Fi credentials and the Blynk **Auth Token** in your sketch.  
5. **Upload and Run:** Upload the modified code to ESP8266. Open **Serial Monitor** to check the connection.  
6. **Monitor via Blynk App:** Add widgets and control ESP8266 from the Blynk mobile app.
