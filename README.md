# 🛡️ Bike Helmet Detection using YOLOv8

This project uses the YOLOv8 nano model to detect whether a person on a bike is wearing a helmet or not. It helps improve road safety through AI-based compliance checking.

## 🔧 Tech Stack
- Python
- Ultralytics YOLOv8
- Google Colab
- Roboflow (for dataset)
- OpenCV

## 📦 Dataset
Custom dataset created using Roboflow, with the following classes:
- With Helmet
- Without Helmet

## 🚀 How to Train (Colab)
```python
from ultralytics import YOLO
model = YOLO('yolov8n.pt')
model.train(data='data.yaml', epochs=10, imgsz=640, batch=8)
```

## 📸 Example Predictions
Located inside `sample_predictions/` folder.

## 🧠 Model Accuracy
Achieved ~85% accuracy on a validation set. Suitable for real-time detection in video or camera feeds.

---

👨‍🎓 **Author:** Yashoraj Singh  
🎓 B.Tech CSE – 3rd Year
