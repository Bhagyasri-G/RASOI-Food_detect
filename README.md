# RASOI Food Detection using YOLOv5

This project uses the YOLOv5 object detection model to detect various food items in the RASOI dataset.

## 📊 Model Info
- Model: YOLOv5s
- Training: ✅ Completed for 25 epochs
- Validation and inference performed on a custom RASOI dataset

## 📁 Inference Results

📦 Final detection output images (with bounding boxes) are stored in a zip file.

🔗 [Click here to download the results (exp.zip)](https://drive.google.com/file/d/1JDIpkFodY-ZvPq-73i3RE_LKmhFgFNu-/view?usp=drive_link)

## 📌 Project Structure
- **Training Results**: `runs/train/exp2/`
- **Inference Output**: `runs/detect/exp/`
- **Weights Used**: `yolov5s.pt` (pre-trained), `best.pt` (custom trained)

## 🚀 How to Run Inference

```bash
python detect.py \
  --weights runs/train/exp2/weights/best.pt \
  --img 640 \
  --source /content/YOLO_DATA/images/val \
  --project runs/detect \
  --name exp \
  --exist-ok
