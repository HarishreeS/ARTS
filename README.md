
![Project Banner](assets/banner.png)

# 🚦 Railway Station Monitoring System

A real-time AI-based monitoring system for railway/metro platforms using YOLOv5 and OpenCV. This project detects passengers near the platform edge, provides alerts when safety lines are crossed, and announces train arrivals via text-to-speech.

---

## 🎯 Features

- 🚨 Detects people crossing the yellow line  
- 📢 Announces train arrival with voice alert  
- 📊 Displays temperature and current time  
- 👤 Login system using a simple GUI  
- 🎥 Processes live or recorded video with bounding boxes  

---

## 🖥️ Demo

#### 🔐 Login Interface and Monitoring UI

| Login Screen | After Login | Detection Ready | Successful Login |
|--------------|-------------|------------------|------------------|
| ![](assets/demo3.png) | ![](assets/demo2.png) | ![](assets/demo1.png) | ![](assets/demo4.png) |

#### 🚉 Real-Time Detection Example

| Platform Detection |
|--------------------|
| ![](assets/demo5.png) |

🎬 **[Watch Demo Video](assets/Demo_Video_ARTS.mp4)**

---

## 🧠 Tech Stack

- **Python 3**
- **YOLOv5s** (via PyTorch Hub)
- **OpenCV** – video processing
- **Tkinter** – GUI interface
- **pyttsx3** – text-to-speech
- **Requests** – dummy temperature API

---

## ⚙️ Setup Instructions

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/railway-station-monitoring.git
   cd railway-station-monitoring
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the project**
   ```bash
   python src/main.py
   ```

---

## 📁 Folder Structure

```text
railway-station-monitoring/
│
├── src/
│   └── main.py                    
│
├── resources/
│   └── yolo_info.md              
│
├── assets/
│   ├── demo1.png               
│   ├── demo2.png                  
│   ├── demo3.png
│   ├── demo4.png
│   ├── demo5.png
│   └── Demo_Video_ARTS.mp4        
│
├── requirements.txt
├── README.md                      
└── .gitignore                     
```

---

## 📄 License

This project is licensed under the **MIT License**. Feel free to use, modify, and share it.
