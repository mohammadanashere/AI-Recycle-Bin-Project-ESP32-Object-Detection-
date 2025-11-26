# AI Recycle Bin  
An AI-powered smart waste segregation system built using **ESP32-CAM** and **TensorFlow Lite**, capable of identifying **Paper, Plastic, and Metal** objects in real time and automatically directing them to the correct bin using servo/stepper motors.

---

## Project Overview
The AI Recycle Bin is designed to solve the problem of manual waste sorting by using **on-device machine learning**.  
It captures images using the ESP32-CAM, classifies the object, and moves the appropriate bin section using motor control.

This project is inspired by the Hackster "AI Audio Classifier Bin" but upgraded to:
- Object detection instead of audio  
- TensorFlow Lite for computer vision  
- Real-time sorting using motors  

---

## Features
- Real-time object classification (Paper, Plastic, Metal)  
- Uses **TensorFlow Lite** model deployed on ESP32-CAM  
- Automatic bin movement via servo/stepper motor  
- Serial communication for debugging  
- Lightweight, fast, and edge-AI optimized  

---

## Tech Stack
- **ESP32-CAM**
- **TensorFlow Lite / TFLite Micro**
- **Edge Impulse / Teachable Machine** (for training)
- **Arduino IDE**
- **Servo / Stepper Motor**
- **Python** (for model training/preprocessing)

---

---

## How It Works
1. Object is placed in front of the ESP32-CAM  
2. Camera captures image  
3. TFLite model classifies object type  
4. Based on the prediction:
   - Servo moves to Paper bin  
   - Servo moves to Plastic bin  
   - Servo moves to Metal bin  
5. Classification result printed via Serial Monitor  

---

## Model Training
- Dataset of Paper, Plastic, and Metal objects trained using Edge Impulse
- Model exported as **TensorFlow Lite**  
- Converted for ESP32-CAM inference  

---

## Future Improvements
- Add more classes (Glass, Organic, E-waste)  
- Add OLED/LCD display  
- Add WiFi-based logging  
- Add auto-lid and safety features  

---

## Project Status
- ✔ Model trained  
- ✔ Classification working on ESP32-CAM  
- ⏳ Motor hardware & logic in progress  

---

## Author
**Mohammad Anas**  
Diploma in Artificial Intelligence & Machine Learning  
(2025)

---

## License
This project is open-source. Feel free to use, modify, and improve it.
