# 👗 Fashion Recommender System

> An **AI-powered web application** that recommends visually similar fashion products using **Deep Learning**, **Computer Vision**, and **Full Stack Web Development**.

---

## 🚀 Overview

**Fashion Recommender System** is an end-to-end AI project that helps users discover visually similar products by uploading an image.  
It combines **TensorFlow (Deep Learning)** with a modern **Next.js (React)** frontend to create an intelligent, interactive recommendation platform.

The system extracts deep visual embeddings using **MobileNetV2**, computes **Cosine Similarity** between product features, and returns the top 5 most similar items — all within seconds.

---

## ✨ Key Features

✅ **AI-Powered Similarity Search**  
- Uses **MobileNetV2** pretrained on ImageNet for fast and accurate image feature extraction.  
- Identifies top 5 visually similar items using **Cosine Distance** and **KNN Search**.

✅ **End-to-End Integration**  
- **Flask Backend** for deep learning inference and similarity computation.  
- **Next.js Frontend** for image upload, API calls, and beautiful UI display.

✅ **Optimized & Scalable**  
- Precomputed embeddings for 44,000+ fashion items.  
- Lightweight and fast inference using **MobileNetV2** instead of heavy ResNet models.

✅ **Real-Time Recommendations**  
- Users upload an image and instantly get top visually similar product suggestions.  

---

## 🧠 Tech Stack

### 💻 Frontend
- **Next.js 14** (React Framework)  
- **Tailwind CSS** for responsive UI  
- **Framer Motion** for smooth animations  
- **Fetch API / Axios** for API calls  

### ⚙️ Backend
- **Flask (Python)** for serving predictions  
- **TensorFlow / Keras** for model inference  
- **Scikit-Learn** for Nearest Neighbors search  
- **OpenCV** for image preprocessing  
- **NumPy & Pickle** for data handling  

### 🧮 Machine Learning & CV
- **Model:** MobileNetV2 (Pretrained on ImageNet)  
- **Pooling:** GlobalMaxPooling2D  
- **Embedding Size:** 1280  
- **Similarity Metric:** Cosine Distance  
- **KNN Search:** 5 nearest results  

---

## 🧩 Architecture

```mermaid
graph TD
A[User Uploads Image] --> B[Next.js Frontend]
B --> C[Flask Backend /predict API]
C --> D[Feature Extraction (MobileNetV2)]
D --> E[Cosine Similarity Search using NearestNeighbors]
E --> F[Top 5 Similar Images Returned as JSON]
F --> G[Frontend Displays Results Grid]

Working Demo

1️⃣ Upload any image (e.g., a watch, t-shirt, or shoe).
2️⃣ Backend extracts features using MobileNetV2.
3️⃣ Cosine similarity is computed against all saved product embeddings.
4️⃣ Frontend displays the top 5 most visually similar items.
