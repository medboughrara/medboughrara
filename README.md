# Hi, I'm Mouhamed Boughrara 👋 

<div align="center">

![Header Banner](https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:0f172a,70:1e1b4b,100:4338ca&height=220&section=header&text=Mouhamed%20Boughrara&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Tech%20Lead%20@%20Qomics%20Startup%20|%20AI%20%26%20Advanced%20Robotics%20|%20Embedded%20Systems&descFontSize=16&descAlignY=62&descAlign=50)

[![GitHub followers](https://img.shields.io/github/followers/medboughrara?style=for-the-badge&logo=github&color=4338ca)](https://github.com/medboughrara)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mouhamed%20Boughrara-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/medboughrara)
[![Email](https://img.shields.io/badge/Email-Contact%20Me-EA4335?style=for-the-badge&logo=gmail)](mailto:126203576+medboughrara@users.noreply.github.com)

</div>

---

### 🧬 System Architecture: Hardware-Software Co-Design

```mermaid
flowchart TD
    subgraph HARDWARE_LAYER ["🔌 Hardware & Embedded Systems"]
        ESP32["ESP32 / Microcontrollers"]
        MKS["MKS Stepper Motor Drivers\n(Sub-micron X/Y/Z Stage)"]
        CAM["Microscope CMOS Camera\n(High-Speed Stream)"]
        PCB["Custom PCB Circuitry\n(KiCad / Altium)"]
    end

    subgraph EDGE_CONTROL ["⚡ Low-Level Control & Firmware"]
        UART["RS485 / UART Protocol Engine"]
        FIRMWARE["C/C++ Motion Controller\n(S-Curve Profile & Safety Limits)"]
    end

    subgraph AI_PIPELINE ["🤖 Computer Vision & AI Core"]
        AF["Z-Autofocus Hill-Climbing Algorithm\n(Tenengrad / Laplacian Variance)"]
        YOLO["YOLO Cell Detection & Segmentation\n(PyTorch / TensorRT / ONNX)"]
    end

    subgraph SOFTWARE_APP ["💻 Web Application & Cloud"]
        FASTAPI["FastAPI Async Backend\n(Python 3.12 / Redis / Postgres)"]
        UI["React & Tailwind Dashboard\n(Real-Time Cytology Visualizer)"]
    end

    ESP32 <-->|UART / RS485| MKS
    PCB --> ESP32
    CAM -->|Raw Video Stream| AF
    AF -->|Focus Metric Feedback| FIRMWARE
    FIRMWARE -->|Step/Dir Commands| ESP32
    CAM --> YOLO
    YOLO --> FASTAPI
    FASTAPI <--> UI
```

---

### 📈 GitHub Activity Graph & Analytics

<div align="center">

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=medboughrara&theme=tokyonight&area=true&hide_border=true)

<br/>

<img src="https://github-readme-stats.vercel.app/api?username=medboughrara&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" width="48%"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=medboughrara&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" width="48%"/>

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=medboughrara&theme=tokyonight&hide_border=true" alt="GitHub Streak" width="48%"/>
<img src="https://github-readme-stats.vercel.app/api/wakatime?username=medboughrara&theme=tokyonight&hide_border=true&layout=compact" alt="WakaTime Stats Chart" width="48%"/>

</div>

---

### 🔄 Control Loop: Real-Time Autofocus & Vision Pipeline

```mermaid
sequenceDiagram
    autonumber
    participant UI as React Frontend
    participant API as FastAPI Backend
    participant CV as OpenCV / YOLO Engine
    participant MCU as ESP32 Firmware
    participant Stage as Z-Axis Motor Stage

    UI->>API: Start Slide Scan Request
    API->>MCU: Move Stage to (X, Y) Position
    MCU->>Stage: Execute Stepper Motor Pulses
    Stage-->>MCU: Arrived at Coordinates

    loop Autofocus Hill-Climbing Loop
        MCU->>Stage: Step Z Axis (Delta Z)
        CV->>CV: Capture Frame & Compute Focus Metric
    end

    CV-->>API: Optimal Z-Plane Located
    API->>CV: Run YOLO Cell Segmentation
    CV-->>UI: Stream Annotated High-Res Cytology Frame
```

---

### 🛠️ Tech Stack & Ecosystem

| Category | Technologies & Tools |
| :--- | :--- |
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white) ![Julia](https://img.shields.io/badge/Julia-9558B2?style=flat-square&logo=julia&logoColor=white) ![VHDL](https://img.shields.io/badge/VHDL-005B94?style=flat-square&logo=hardware&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) |
| **Embedded & Microcontrollers** | ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white) ![STM32](https://img.shields.io/badge/STM32-03234C?style=flat-square&logo=stmicroelectronics&logoColor=white) ![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white) ![RS485](https://img.shields.io/badge/RS485%20%2F%20UART-FF6F00?style=flat-square&logo=connectify&logoColor=white) |
| **PCB Design & CAD** | ![KiCad](https://img.shields.io/badge/KiCad-314185?style=flat-square&logo=kicad&logoColor=white) ![Altium](https://img.shields.io/badge/Altium-A20000?style=flat-square&logo=altiumdesigner&logoColor=white) ![EasyEDA](https://img.shields.io/badge/EasyEDA-0066FF?style=flat-square&logo=easyeda&logoColor=white) ![EAGLE](https://img.shields.io/badge/EAGLE-005B94?style=flat-square&logo=autodesk&logoColor=white) |
| **AI, Computer Vision & Sim** | ![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat-square&logo=ultralytics&logoColor=black) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![NVIDIA Isaac Sim](https://img.shields.io/badge/Isaac%20Sim-76B900?style=flat-square&logo=nvidia&logoColor=white) ![Webots](https://img.shields.io/badge/Webots-FF0000?style=flat-square&logo=cyberbotics&logoColor=white) |
| **Backend & Cloud** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |

---

### ⏱️ Automated WakaTime Stats

<!--START_SECTION:waka-->
<!--END_SECTION:waka-->

---

### 🌟 Featured Projects

<details>
<summary><b>🔬 SmartCytoScan / QVision System (Click to expand)</b></summary>
<br/>

AI-Powered Automated Cytology Microscope & Scanner. Integrates high-precision stepper stage motion control, sub-micron Z-autofocus hill-climbing, ESP32 hardware interfaces, real-time slide cell detection using YOLO, and asynchronous FastAPI backend.

```mermaid
graph LR
    A[Cytology Slide] --> B[High-Resolution Camera]
    B --> C[Focus Evaluation Engine]
    C --> D[YOLO Cell Segmentation]
    D --> E[Diagnostic Report Generation]
```
</details>

<details>
<summary><b>⚡ High-Precision RS485 Motor Controller Firmware (Click to expand)</b></summary>
<br/>

Embedded C++ and Python communication stack for MKS/TMC motor drivers, implementing fast S-curve velocity profiling, limit switch safety bounds, and emergency stopping mechanisms over RS485/UART protocols.
</details>

---

<div align="center">

**[github.com/medboughrara](https://github.com/medboughrara)** • *Hardware-Software Co-Design & Robotics AI*

</div>
