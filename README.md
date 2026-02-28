# Truck Loading & Sack Movement Detection (Computer Vision Project)

This project demonstrates a basic computer vision pipeline to monitor loading and unloading activity from truck videos.  
The system detects workers, tracks their movement, and estimates sack transfer events based on spatial movement near the truck.

---

## 🚀 Project Objective
To build a simple ML/CV pipeline that can:
- Process logistics videos
- Detect and track workers
- Identify loading/unloading motion near the truck
- Estimate sack movement count
- Generate annotated output videos

---

## 🧠 Approach

Since sack labels were not available, the system approximates sack transfer by:

1. Detecting people and trucks using a pretrained YOLOv8 model  
2. Tracking workers across frames using ByteTrack  
3. Defining a truck loading zone  
4. Counting workers crossing the boundary near the truck  
5. Producing an annotated output video with counts

---

## 🛠️ Tech Stack

- Python  
- OpenCV  
- YOLOv8 (Ultralytics)  
- ByteTrack Tracking  
- Google Colab  

---

## 📂 Project Workflow

1. Upload videos to Google Drive  
2. Run detection and tracking in Colab  
3. Apply spatial filtering near the truck  
4. Count loading events using boundary logic  
5. Export annotated output video  

---

## 📊 Output

- Bounding boxes for detected workers  
- Tracking IDs for each person  
- Loading zone visualization  
- Estimated sack movement count  
- Processed demo video output  

---

## 📌 Use Cases

- Warehouse monitoring  
- Truck loading supervision  
- Industrial automation demos  
- Logistics analytics research  
---

## 📁 Video Samples

The videos used for this project can be accessed here:

🔗 **Google Drive Link:**  
[https://drive.google.com/drive/folders/1UI03OsuuQhoSprJ3iCVBDCpd7-hnbEgK?usp=sharing]

*(Includes processed outputs used for testing the pipeline.)*

---
---

## ✍️ Author

[Dhairya Saigal]

---
