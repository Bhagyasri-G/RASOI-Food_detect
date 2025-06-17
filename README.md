# 🍽️ RASOI Food Detection using YOLOv5

This project uses the YOLOv5 object detection model to detect various food items from the RASOI dataset.

## 📊 Model Info
- Model: YOLOv5s
- Epochs: 25
- Batch Size: 16
- Image Size: 640×640
- Framework: PyTorch

## 📁 Project Structure
- **Training Results**: `runs/train/exp2/`
- **Inference Output**: `runs/detect/exp/`
- **📦 Download Inference ZIP**: [Click here to download `exp.zip`](https://drive.google.com/file/d/1Lqxepajqmqa2EMX59xrOXkkRheuWiSMP/view?usp=drive_link)

## 🚀 How to Run Inference

```bash
python detect.py \
  --weights runs/train/exp2/weights/best.pt \
  --img 640 \
  --source /content/YOLO_DATA/images/val \
  --project runs/detect \
  --name exp \
  --exist-ok
