# 💄 Virtual Makeup Application using OpenCV & Dlib

A computer vision–powered application that applies **virtual makeup** (lipstick, eyeshadow, and blush) to faces in images using facial landmark detection and image masking techniques. Built using **OpenCV**, **Dlib**, and **NumPy**, this project simulates cosmetic effects in a realistic and dynamic way.

> 👁️ Try-before-you-buy virtual makeup, real-time augmentation, and image enhancement using deep learning and classic CV — all in one project.

---

## 🎯 Project Objective

To design a virtual makeup system that:
- Detects facial features using **Dlib's 68-point landmark detector**
- Applies cosmetic effects like lipstick, eyeshadow, and blush using **image masks and blending**
- Produces a natural, smooth, and realistic enhancement of facial images


## 🧠 What I Learned

This project taught me how to:
- Use **facial landmark detection** to identify regions of interest (lips, eyes, cheeks)
- Design and apply **custom color masks** to selected facial areas
- Blend color effects using **Gaussian blur** and `cv2.addWeighted` for realism
- Perform **SSIM-based evaluation** to compare generated images to real makeup
- Automate image enhancement pipelines and analyze model accuracy using classification metrics
- Handle real-world challenges like lighting variation, occlusion, and facial shape diversity

---

## 🛠 Tech Stack

| Tool            | Purpose                                      |
|------------------|----------------------------------------------|
| Python 3.10       | Main programming language                   |
| OpenCV            | Image processing & visual effects           |
| Dlib              | Facial detection & 68-point landmark model  |
| NumPy             | Mask creation & image array manipulation    |
| scikit-learn      | Evaluation metrics (Accuracy, Precision)    |
| SSIM (scikit-image) | Image similarity comparison               |
| Google Colab      | Notebook execution and demonstration        |

---

## 🔍 How It Works

### 📌 Facial Landmark Detection
- Uses `shape_predictor_68_face_landmarks.dat` from Dlib
- Detects key points for:
  - **Lips**: landmarks 48–67
  - **Eyes**: landmarks 36–41 (left), 42–47 (right)
  - **Cheeks**: landmarks 1–5 (left), 11–15 (right)

### 💄 Makeup Effects
| Effect     | Area   | Color (BGR)       | Technique             |
|------------|--------|------------------|------------------------|
| Lipstick   | Lips   | (170, 8, 180)     | Color mask + blur      |
| Eyeshadow  | Eyes   | (130, 20, 30)     | Polygon mask + blur    |
| Blush      | Cheeks | (200, 22, 12)     | Circle mask + blending |

### 🧪 Evaluation
- **SSIM Score** used to compare virtual makeup vs. real makeup
- **Accuracy, Precision, Recall, F1-score** calculated from SSIM thresholds
- Automated processing of multiple face images
---

## 🔍 Challenges Faced

- 🎯 Accurate landmark detection under varied lighting and poses
- 🎨 Achieving realistic blending of makeup without harsh edges
- 📏 Dealing with variation in face shapes, skin tones, and feature positions
- 🤖 Balancing the intensity of multiple simultaneous effects (e.g., lipstick + blush)

---

## 🧪 Applications

- 🛍️ **Virtual try-on** for cosmetic e-commerce
- 📸 **Photo editing** and AR selfie apps
- 🎥 **Video conferencing** real-time enhancements
- 🎬 **Film & TV** for rapid makeup previews
- 💄 **Beauty industry** for personalized product recommendation

---

## 📊 Results

| Metric     | Value   |
|------------|---------|
| SSIM Avg.  | 0.87+   |
| Accuracy   | 91.5%   |
| Precision  | 90.2%   |
| F1 Score   | 90.7%   |

✅ Makeup results were **visually realistic** and **quantitatively aligned** with real makeup images.


This project demonstrates:
- **Computer vision expertise**: Face detection, image masking, visual blending
- **Applied problem-solving**: Real-world AR/beauty use case
- **Data evaluation skills**: SSIM + ML classification metrics
- **Code quality**: Clean structure, modular functions, scalable pipeline
- **Creativity**: Simulating physical makeup through digital artistry

