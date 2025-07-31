# 📚 YOLO Model Information

This project uses the **YOLOv5s** (YOLOv5 Small) model from the [Ultralytics YOLOv5 repository](https://github.com/ultralytics/yolov5), loaded via PyTorch Hub.

---

## 🔍 Model Details

- **Model:** YOLOv5s (small, pretrained on COCO dataset)
- **Loaded Using:**
  ```python
  model = torch.hub.load('ultralytics/yolov5', 'yolov5s')

Classes Detected: 80 (COCO dataset), including person, train, car, etc.

Framework: PyTorch (no separate weights required if online)

🛠️ How It's Used in This Project
In the script (main.py), YOLOv5 is used to detect objects in each video frame:

results = model(frame)
detections = results.xyxy[0]  # Each row: [x1, y1, x2, y2, confidence, class]

We use this to:

Detect people (label == 'person') and determine if they cross the yellow safety line

Detect trains to trigger automated announcements

📦 Why YOLOv5s?
   ⚡ Fast Inference: Optimized for real-time detection

    🎯 Accurate Enough: Balances speed and accuracy for small to mid-scale projects

    🧩 Easy Integration: Works directly with PyTorch and supports GPU/CPU

🧠 Future Improvements (Optional)
You can fine-tune YOLOv5 on your own dataset (e.g. platform footage) to improve accuracy for edge cases:

    Prepare a labeled dataset (YOLO format)

    Train using the Ultralytics training CLI or script

    Replace yolov5s with a custom .pt weight file

Learn more here: YOLOv5 Custom Training Guide

🔗 Resources
   🔗 Ultralytics GitHub

   🧾 YOLOv5 Docs

   📄 COCO Class List

   📚 YOLOv5 Custom Training