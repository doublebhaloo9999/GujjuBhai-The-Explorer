# 🗺️ GujjuBhai the Explorer: Interactive Geography Learning Tool

**GujjuBhai the Explorer** is a smart educational toy designed to teach the geography and culture of Gujarat to rural students. It combines a physical wooden puzzle with digital interactivity using NFC technology and Audio feedback.

## 🌟 Key Features
* **Interactive Learning:** Students scan physical flashcards to hear audio clues about districts.
* **Tactile Puzzle:** A laser-cut wooden map for hands-on spatial understanding.
* **Audio Feedback:** Uses a DFPlayer Mini to play descriptions, folklore, and facts.
* **Visual Feedback:** RGB LED indicates scanning status (Success/Error).
* **Portable Power:** Powered by a single 18650 Li-Ion battery with a custom boosted 5.1V rail.

## 🛠️ Hardware Components
* **Microcontroller:** ESP32 DevKit V1 (Dual-Node Architecture via ESP-NOW)
* **NFC Reader:** PN532 (High-Speed UART Mode)
* **Audio:** DFPlayer Mini + 3W Speaker
* **Power:** TP4056 (Charging) + MT3608 (Boost Converter) + 18650 Battery
* **Interface:** RGB LED + Volume Push Buttons

## 🔌 Circuit Diagram
*(You can view the full circuit diagram in the `Circuit` folder)*

1.  **NFC (PN532):** Connected to Serial 2 (GPIO 16/17).
2.  **Audio (DFPlayer):** Connected to Serial 1 (GPIO 26/27).
3.  **Power:** Boosted 5.1V rail with a 470uF capacitor for bass stability.

## 🚀 How to Run
1.  **Hardware:** Assemble the circuit as per the diagram.
2.  **Libraries:** Install `Adafruit_PN532`, `DFRobotDFPlayerMini`, and `Blynk` (optional) in Arduino IDE.
3.  **Upload:** Flash the code located in the `Code/` folder to the ESP32.
4.  **SD Card:** Format SD card to FAT32 and add MP3 files in a folder named `mp3` (files named `0001.mp3`, `0002.mp3`, etc.).

## 🔮 Future Improvements
* Bluetooth Companion App for teachers.
* OTA (Over-the-Air) updates for adding new districts wirelessly.
* Deep Sleep mode for longer battery life.

## 📄 Project Report
For detailed technical specifications and the full project report, please check the `Docs/` folder.

---
*Created by [Your Name]*
