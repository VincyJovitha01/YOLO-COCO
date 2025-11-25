# YOLO Object Detection – Streamlit Deployment

## 1. Project Title
**Real-Time Object Detection Using YOLO and Streamlit**

---

## 2. Abstract / Introduction

This project implements a real-time object detection system using the **YOLO (You Only Look Once)** model trained on the **COCO dataset**.

The objective is to build an end-to-end detection pipeline that:

- Runs locally using a **Conda environment**
- Executes in **Visual Studio Code**
- Performs object detection on **images, videos, and webcam input**
- Deploys through an interactive **Streamlit web UI**

The YOLO model identifies **80+ object classes** with high accuracy and real-time performance, enabling applications such as surveillance, analytics, and intelligent automation.

---

## 3. Dataset & YOLO Model Details (COCO)

### **COCO Dataset (Common Objects in Context)**

- Large-scale dataset for object detection, segmentation, and image captioning  
- Contains **80 object categories** such as humans, vehicles, animals, furniture, etc.  
- Used to pretrain YOLO models for high accuracy and robustness  

### **YOLO Model Used**

- Model Type: **YOLO (YOLOv8 / YOLOv5)**  
- Framework: **Ultralytics**  
- Pretrained on COCO  
- Supports real-time detection on CPU/GPU  

**Model Outputs:**
- Bounding Boxes  
- Class Labels  
- Confidence Scores  

---

## 4. Environment Setup

This project must be executed **locally** using **Conda** and **Visual Studio Code (VS Code)**.

### **Step 1 — Create Conda Environment**
```
conda create -n yolo_env python=3.10 -y
conda activate yolo_env
```

### **Step 2 — Install Dependencies (CPU version)**
```
pip install ultralytics
pip install streamlit opencv-python pillow numpy
```
### **Step 3 — (Optional) GPU Installation**
```
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install ultralytics
pip install streamlit opencv-python pillow numpy
```
## 5.Run the Streamlit Application
```
streamlit run app.py
```
## Output:
<img width="1838" height="404" alt="image" src="https://github.com/user-attachments/assets/720bfee1-6ea0-4d94-b8b0-9766e8d6c95c" />

<img width="1827" height="432" alt="image" src="https://github.com/user-attachments/assets/22f00dd2-970a-41ed-aa6b-834b67904c48" />

<img width="1882" height="858" alt="image" src="https://github.com/user-attachments/assets/b71bdfd1-555f-47bc-8e7d-ed77c3806bcc" />

## Result:

The YOLO model successfully detected objects in images, videos, and webcam input using the Streamlit application. The system produced clear bounding boxes and labels for various COCO classes and worked smoothly on my local machine using the Conda environment in VS Code. The app launched correctly with `streamlit run app.py` and displayed accurate results for all tested inputs.
