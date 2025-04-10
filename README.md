# 🧠 AI Vision System using ESP32-CAM & OpenAI GPT-4o

This project demonstrates a compact **AI Vision System** built using the ESP32-CAM module and OpenAI's GPT-4o Vision API. It captures real-world images, encodes them into Base64, and sends them over the internet to OpenAI for analysis. The API’s intelligent response is displayed on an OLED screen with smooth scrolling and buzzer-based feedback.

Although it runs on microcontroller hardware, the project heavily focuses on **cloud integration, real-time image processing, and embedded user interfaces** — highlighting software engineering skills like API communication, memory-constrained processing, and system design.

---

## 🚀 Key Features

- 📷 **Image Capture** using ESP32-CAM  
- 🔐 **Base64 Encoding** for efficient image transmission  
- ☁️ **API Integration** with OpenAI GPT-4o Vision endpoint  
- 🧠 **AI-Powered Analysis** of real-world captured images  
- 📺 **OLED Display Output** with scrolling text  
- 🔊 **Buzzer Feedback** for user acknowledgment  
- 📡 **Wi-Fi Connectivity** for internet-enabled vision tasks  

---

## 🛠️ Tech Stack

| Component | Description |
|----------|-------------|
| **ESP32-CAM** | Low-cost AI-enabled microcontroller with onboard camera |
| **Arduino IDE** | Development environment used for coding and uploading firmware |
| **OpenAI GPT-4o Vision API** | Provides image understanding and semantic analysis |
| **Adafruit SSD1306 + GFX Library** | Used for controlling OLED display output |
| **Base64 Encoding** | Translates image bytes for cloud-safe transmission |
| **ArduinoJson** | Parses and extracts AI responses from API replies |

---

## 📦 Libraries Used

Ensure you have the following versions (or newer) installed:

- **ESP32 Board Package**: `3.0.0`  
- **Adafruit SSD1306**: `2.5.13`  
- **Adafruit GFX Library**: `1.11.11`  
- **ArduinoJson**: `7.1.0`  
- **Base64**: *(Built-in with ESP32 board support)*

---

## ⚙️ How It Works

1. **Boot & Connect**: ESP32 connects to Wi-Fi on boot.  
2. **Capture**: An image is captured through the onboard camera.  
3. **Encode**: The image is encoded into Base64 format.  
4. **Transmit**: The encoded image is sent to OpenAI's GPT-4o Vision API.  
5. **Analyze**: OpenAI returns a natural language description of the image.  
6. **Display**: The description is shown on the OLED screen with auto-scrolling.  
7. **Feedback**: A buzzer provides an audio cue when a response is received.

---

## 🔧 Setup Instructions

1. **Install Arduino IDE** (v2.3.2 recommended)  
2. **Add ESP32 Boards**:
   - Go to `File > Preferences` and add this URL under **Additional Board Manager URLs**:
     ```
     https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
     ```
3. **Install Required Libraries** via Library Manager:
   - Adafruit GFX
   - Adafruit SSD1306
   - ArduinoJson
4. **Open the Code** and update:
   - Your Wi-Fi credentials
   - Your OpenAI API key
5. **Connect the ESP32-CAM**:
   - Board: `AI Thinker ESP32-CAM`
   - Select the correct port and upload the code
6. **View Output**:
   - Watch the OLED display the AI-generated result
   - Check the Serial Monitor for logs and Base64 data

---

## 📷 Example Use Cases

- Real-time object or scene recognition  
- Edge AI demonstrations with minimal power usage  
- IoT integration with cloud-based computer vision  
- Educational tool for understanding AI inference pipelines

---

## 💡 Why This Project?

While it's hardware-backed, this project demonstrates **cloud-centric software design**, including:

- Efficient API handling under low memory conditions  
- Asynchronous data transfer and UI feedback  
- Use of advanced AI models via REST API  
- Real-time UX management on resource-constrained devices

---

## 🧪 Tested On

- ESP32-CAM AI Thinker Module  
- Arduino IDE 2.3.2  
- Wi-Fi network with internet access  
- 128x64 I2C OLED Display

---

## 🛡️ License

This project is open-source and MIT-licensed.

