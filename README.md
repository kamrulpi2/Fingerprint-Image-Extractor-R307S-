# 🔍 Fingerprint Image Extractor (ESP32 + R307 + Python)

This project captures raw fingerprint images from an **R307 fingerprint sensor** using an **ESP32**, then converts them into a **PNG image using Python**.

---

## ✨ Features

* Capture raw fingerprint image
* Transfer data via Serial (HEX stream)
* Decode R307 packets
* Convert to grayscale PNG
* Auto-save to Downloads folder

---

## 🧰 Hardware Required

* ESP32
* R307 Fingerprint Sensor
* Jumper Wires

---

## 🔌 Wiring (ESP32 ↔ R307)

| R307 | ESP32        |
| ---- | ------------ |
| VCC  | 5V           |
| GND  | GND          |
| TX   | GPIO16 (RX2) |
| RX   | GPIO17 (TX2) |

---

## ⚙️ ESP32 Setup

1. Install Arduino IDE
2. Install libraries:

   * Adafruit Fingerprint Sensor Library
3. Upload code from:

   ```
   esp32/fingerprint_capture.ino
   ```

---

## 🐍 Python Setup

### Install dependencies:

```
pip install -r requirements.txt
```

### Run script:

```
python python/extract_fingerprint.py
```

---

## 📁 Output

* Saved automatically to:

```
C:/Users/YourName/Downloads/fingerprint_scan.png
```

---

## ⚠️ Notes

* Close Arduino Serial Monitor before running Python
* Set correct COM port in Python script

---

## 📸 Demo Workflow

1. Place finger on sensor
2. ESP32 reads image
3. Data sent to PC
4. Python converts to PNG

---

## 📜 License

MIT License

---

## 👨‍💻 Author

Kamrul (BUBT AgroDoctor Team 🚀)

https://www.alldatasheet.com/datasheet-pdf/pdf/1756584/GROW/R307.html
<img width="891" height="511" alt="image" src="https://github.com/user-attachments/assets/2bd97623-1dab-4d75-b183-c820452fb786" />
<img width="332" height="392" alt="image" src="https://github.com/user-attachments/assets/bd4ce0aa-c3a2-460c-b79d-3b670a611307" />



