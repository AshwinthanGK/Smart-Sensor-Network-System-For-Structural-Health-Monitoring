# Smart Sensor Network System for Structural Health Monitoring (SHM)

**Authors:** N. Shadhurshan, S. Sarusan, G.K. Ashwinthan, M.B. Dissanayake, H.A.D. Samith Buddika  
**Departments:** Electrical & Electronic Engineering / Civil Engineering, University of Peradeniya  
**Correspondence:** e20372@eng.pdn.ac.lk | +94 772747187  

---

## Project Overview

Structural health monitoring (SHM) is critical for ensuring the safety, durability, and serviceability of civil infrastructures. Cracks in concrete often indicate early deterioration and potential structural failures. Traditional methods like visual inspection are **time-consuming, subjective, and hard to scale**, while purely sensor-based approaches lack precise spatial localization.

This project presents a **hybrid framework** combining:

1. **Sensor-driven monitoring** using **ESP32-based LoRa nodes with custom capacitive sensors**  
2. **Machine learning analysis** (SVM, MLP, XGBoost) for crack classification and severity prediction  

The framework achieves **robust, accurate, and scalable monitoring**, suitable for real-time SHM under variable environmental conditions.

---

## Key Features

### 1. Sensor Network
- **ESP32 microcontrollers** as sensor nodes  
- **LoRa SX1278 modules** for long-range, low-power wireless communication  
- Collect **capacitive, temperature, humidity, and thickness data** from concrete structures  
- Master node aggregates and processes data for real-time analysis  

### 2. Capacitive Sensor-Based Crack Detection
- **Custom parallel-plate capacitive sensors** embedded in concrete at crack locations  
- Detect subtle changes in dielectric properties due to crack formation  
- Integrated with environmental sensors for accurate compensation  

### 3. Machine Learning Analysis
- **Support Vector Machine (SVM):** High accuracy for small-to-medium datasets  
- **Multi-Layer Perceptron (MLP):** Captures nonlinear relationships among sensor features  
- **XGBoost:** Efficient, scalable, robust to noisy multi-sensor data  
- Evaluated with **accuracy, precision, recall, F1-score, and ROC/AUC metrics**  

---

## System Architecture

**Stage 1 – Sensor-Based Continuous Monitoring**
1. Deploy capacitive sensors at localized cracks  
2. Collect capacitance, temperature, humidity, and thickness data continuously  
3. Transmit readings via LoRa to master node  

**Stage 2 – ML-Based Crack Classification**
1. Train SVM, MLP, and XGBoost models on collected sensor data  
2. Predict crack presence and severity  
3. Integrate sensor data for high-accuracy assessment  

---

## Hardware Components

- **ESP32** microcontroller boards  
- **LoRa SX1278** wireless modules  
- **Custom parallel-plate capacitive sensors**  
- **DHT11 sensors** for temperature and humidity  

---

## Software & Tools

- **Programming:** Python, C/C++ (Arduino/ESP32)  
- **Embedded Development:** Arduino IDE, PlatformIO  
- **ML & Deep Learning:** TensorFlow, Keras, Scikit-learn, XGBoost, PyTorch  
- **Data Visualization:** Matplotlib, Seaborn  
- **Communication Protocols:** LoRa  

---

## Results & Findings

- **Sensor-based crack classification:**  
  - **SVM:** 91.88% accuracy, highly effective for smaller datasets  
  - **MLP:** 86.57% accuracy, flexible for nonlinear patterns  
  - **XGBoost:** 89.68% accuracy, fastest convergence (2s), ideal for real-time deployment  
- Integration of sensor data allows robust monitoring under variable environmental conditions  

---

## Future Work

- Deploy multiple sensor modules for large-scale structures  
- Integrate with **cloud-based monitoring and dashboards** for real-time alerts  
- Expand ML models to predict crack growth and long-term structural health  

---

## Team Members

- **N. Shadhurshan** – Electrical & Electronics Engineering, University of Peradeniya  
- **S. Sarusan** – Electrical & Electronics Engineering, University of Peradeniya  
- **G.K. Ashwinthan** – Electrical & Electronics Engineering, University of Peradeniya  

---

## Supervisors

- **Prof. (Mrs.) Maheshi B. Dissanayake**  
  Senior Lecturer, Dept. of Electrical & Electronic Engineering, University of Peradeniya, Sri Lanka  
  B.Sc. Eng. (First Class Honours, Electrical & Electronic Engineering), University of Peradeniya, 2006  
  Ph.D. in Electronic Engineering, University of Surrey, UK, 2010  

- **Dr. H.A.D. Samith Buddika, PhD, CEng., MIE(SL), MSSE(SL), Green AP**  
  Senior Lecturer, Dept. of Civil Engineering, University of Peradeniya, Sri Lanka  
  Chartered Engineer – Institute of Engineers, Sri Lanka  
  Corporate Member – Society of Structural Engineers, Sri Lanka  

---

## License

This project is conducted as a **Final Year Project at the University of Peradeniya**.

---



