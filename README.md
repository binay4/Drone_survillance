## 🚁 AI-Powered Drone Surveillance System using Deep Learning

This project implements an intelligent drone surveillance system capable of automatically detecting persons and faces in real-time drone video.
It combines cutting-edge deep learning models with computer vision to ensure robust security in outdoor environments.

📌 Project Motivation

Traditional CCTV security suffers from:

Limited field of view

High manpower requirement

Poor performance in outdoor lighting

No aerial tracking ability

Drones provide mobility, but require AI-based automation to detect threats.

Our solution improves surveillance efficiency by detecting humans and faces from drone footage using a deep-learning pipeline.

✨ Key Features

✔ Real-time person detection using YOLOv5
✔ Robust face detection using MTCNN
✔ Performance metrics: Precision, Recall, FPS, F1-Score
✔ Two-phase evaluation: Baseline vs Optimized
✔ Designed for outdoor drone footage

## 🔍 Technologies Used

| Category | Technology |
|---------|------------|
| Language | Python |
| Vision Framework | OpenCV |
| Deep Learning | PyTorch |
| Object Detection | YOLOv5 |
| Face Detection | MTCNN |
| Deployment | Google Colab / Edge GPU Hardware |

## 📊 System Architecture

[Drone Video] → [Frame Processing] → [YOLOv5 - Person Detection] → [MTCNN - Face Detection] 
              → [Metrics + Visualization] → [Final Output]


🧪 Performance Evaluation

Evaluation performed on the same drone video for fairness.

🔹 Before Optimization (Baseline — Haar Cascade)

Only detects frontal faces

No person detection

Poor drone adaptability

🔹 After Optimization (YOLOv5 + MTCNN)

Detects both persons + faces

Handles drone footage lighting, angles

FPS tracking for real-time latency monitoring

## 📌 Output Visualization Comparison

| Feature | Baseline (Haar Cascade) | Optimized (YOLOv5 + MTCNN) |
|--------|------------------------|----------------------------|
| Person Detection | ❌ Not Supported | ✔ Yellow bounding box |
| Face Detection | ✔ Only frontal faces | ✔ Multi-angle + accurate |
| FPS Overlay | ❌ Not shown | ✔ Real-time FPS display |
| Outdoor Performance | ❌ Misses most faces | ✔ Reliable + robust |
| Tech Type | Classical Computer Vision | Deep Learning |

## 📈 Performance Results

| Metric | Baseline Model | Optimized Model | Improvement |
|--------|----------------|----------------|-------------|
| Precision | 1.00 | 1.00 | Same |
| Recall | 0.04 | 0.30 | **+650% 🚀** |
| F1-Score | 0.08 | 0.46 | **+475% 🚀** |
| Avg FPS (CPU) | 6.61 | 1.29 | Deep models → heavier compute |



🛠 How to Run

1️⃣ Open Google Colab

2️⃣ Upload script + video

3️⃣ Mount Google Drive to access test videos

4️⃣ Update video_path in code

5️⃣ Run the notebook cells in order




🚀 Future Scope

Add face recognition (Inception-ResNet)

Multi-person tracking (DeepSORT)

Real-time intrusion alerts

Autonomous drone navigation integration
