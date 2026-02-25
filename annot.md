# Image Annotation Using CVAT (Beginner Level)

**Prepared by:**  

[Renann G. Baldovino, PhD](https://www.dlsu.edu.ph/colleges/gcoe/academic-departments/manufacturing-engineering-management/faculty-profile/renann-baldovino/)  
**[Department of Manufacturing Engineering and Management, De La Salle University (DLSU)](https://www.dlsu.edu.ph/colleges/gcoe/academic-departments/manufacturing-engineering-management/)**

## Learning Objectives
After completing this lab, you should be able to:
1. Understand the purpose of image annotation in machine learning  
2. Create a task in CVAT  
3. Define labels correctly  
4. Annotate images using bounding boxes  
5. Export annotations in YOLO or COCO format  

## What is CVAT?
[CVAT](https://github.com/opencv/cvat) (Computer Vision Annotation Tool) is an open-source, web-based annotation platform used to label images and videos for AI and computer vision applications. It is commonly used for:
- Object Detection (Bounding Boxes)
- Image Segmentation (Polygons)
- Classification (Tags)
- Keypoint Detection

# PART 1: Accessing CVAT
### Step 1: Open CVAT
Go to: https://app.cvat.ai

### Step 2: Create an Account or Log In

# PART 2: Creating a New Annotation Task
### Step 1: Create Task
Click:

> **Create New Task**

### Step 2: Fill in Task Details

| Field | What to Enter |
|--------|--------------|
| Task Name | Example: `Student_Lab_Annotation` |
| Project | Leave blank (for beginners) |
| Labels | Define your object classes |

# PART 3: Creating Labels
Labels define what objects you want to detect.

### Example (Medical or General Dataset)
Add the following labels:

| Label Name | Shape Type |
|------------|------------|
| Object_A | Rectangle |
| Object_B | Rectangle |

👉 Click **Add Label**  
👉 Enter label name  
👉 Select **Rectangle**  
👉 Click **Done**

💡 For beginners, use **Rectangle** only.

# 📂 PART 4: Upload Images

1. Click **Select Files**
2. Upload at least 5–10 images
3. Click **Submit & Open**

You will now enter the annotation workspace.

# PART 5: Annotating Images (Bounding Boxes)
### Step-by-Step:
1. Select the **Rectangle Tool**
2. Choose your label (e.g., Object_A)
3. Click and drag around the object
4. Press **Enter** to confirm
⚠ Important: Always press **Enter**, or the annotation will not be saved.

# Navigating Images
- Press **N** → Next image  
- Press **P** → Previous image  
- Use mouse scroll to zoom  

# PART 6: Saving and Exporting
### To Export:
1. Go back to Task page
2. Click **Actions**
3. Select **Export Task Dataset**
4. Choose format:
   - YOLO (for object detection models)
   - COCO (common research format)

# Annotation Best Practices
✔ Draw tight bounding boxes  
✔ Be consistent across images  
✔ Zoom in for small objects  
✔ Use the correct label  

# BEGINNER LAB ACTIVITY
# Lab Title: Basic Object Detection Annotation Using CVAT

## Objective:
Annotate a small image dataset using bounding boxes and export it in YOLO format.

## Dataset Requirement
Download or prepare:
- 10–20 images containing at least 2 object types  
  (Example: Cats & Dogs OR Medical: Normal & Pneumonia X-rays)

# Step-by-Step Laboratory Procedure
## Step 1: Login to CVAT
Go to: https://app.cvat.ai

## Step 2: Create New Task
- Task Name: `Lab1_ObjectDetection`
- Add Labels:
  - Class1
  - Class2
- Shape Type: Rectangle
Click **Submit**

## Step 3: Upload Images
- Click **Select Files**
- Upload your dataset
- Click **Submit & Open**

## Step 4: Annotate All Images
For each image:
1. Select Rectangle tool  
2. Choose correct label  
3. Draw bounding box  
4. Press Enter  
5. Move to next image  
Repeat until all images are annotated.

## Step 5: Review Annotations
- Check for missing objects  
- Ensure boxes are tight  
- Confirm correct labels  

## Step 6: Export Dataset
1. Go back to Task
2. Click **Actions → Export Task Dataset**
3. Select **YOLO format**
4. Download the ZIP file

# Optional Medical Informatics Version
For a health analytics adaptation:
### Labels:
- Pneumonia
- Normal

Students can:
- Annotate chest X-rays
- Export COCO format
- Use the dataset for model training in Python (e.g., CNN or YOLO)
