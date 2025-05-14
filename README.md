# 🎯 Gunny Bag Detection using YOLOv8 (Windows)

This project uses the YOLOv8 object detection model to perform **real-time gunny bag detection** on video files. It is designed to work seamlessly on **Windows**, using Python and OpenCV.

---

## 📦 Features

- 🎥 Real-time detection on video (`data/video1.mp4`)
- 🧠 YOLOv8 inference (Ultralytics API)
- 📏 Bounding boxes with labels and detection speed
- 💻 Windows command-line compatible

---

## 🛠️ Requirements

- Python 3.10 (recommended)
- Git
- OpenCV with GUI support
- GPU (optional but recommended)

---

## 📁 Folder Structure

GunnyBagCounter/
├── Gunny-Bags-Counting/
│ ├── gunny_test.py # Real-time video detection script
│ ├── yolov8n.pt # YOLOv8 pretrained model
│ ├── data/
│ │ └── video1.mp4 # Test video
│ ├── runs/ # Output directory for YOLO results
│ └── README.md # You are here

yaml
Copy code

---

## 🚀 Setup & Run (Windows CMD)

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YourUsername/Gunny-Bags-Counting.git
cd Gunny-Bags-Counting
2️⃣ Create Virtual Environment
bash
Copy code
python -m venv venv
venv\Scripts\activate
3️⃣ Install Dependencies
bash
Copy code
pip install --upgrade pip
pip install ultralytics opencv-python numpy
4️⃣ Place Files
Place yolov8n.pt (or best.pt) in the same folder.

Place video1.mp4 inside the data/ folder.

5️⃣ Run the Detection Script
bash
Copy code
python gunny_test.py
👁️ Press Q to quit the video window.

📜 Sample Output
bash
Copy code
0: 384x640 3 persons, 48.5ms
Speed: 1.2ms preprocess, 48.5ms inference, 1.3ms postprocess per image
