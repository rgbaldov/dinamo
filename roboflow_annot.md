# Image Annotation Using CVAT

**Prepared by:**
[Renann G. Baldovino, PhD](https://www.dlsu.edu.ph/colleges/gcoe/academic-departments/manufacturing-engineering-management/faculty-profile/renann-baldovino/)  
**[Department of Manufacturing Engineering and Management, De La Salle University (DLSU)](https://www.dlsu.edu.ph/colleges/gcoe/academic-departments/manufacturing-engineering-management/)**

## Learning Objectives
After completing this lab, you should be able to:
1. Understand the purpose of image annotation in machine learning  
2. Create a project in Roboflow  
3. Define labels correctly  
4. Annotate images using bounding boxes  
5. Export annotations in YOLO or COCO format  

## What is Roboflow?
[Roboflow](https://roboflow.com/) is a web-based platform that allows users to upload, annotate, manage, and export datasets for computer vision projects. It is commonly used for:
- Object Detection (Bounding Boxes)
- Instance Segmentation
- Image Classification
- Dataset Augmentation
- Model Training & Deployment
Roboflow is beginner-friendly and widely used in academic and research settings.

# PART 1: Creating a Roboflow Account
### Step 1: Open Roboflow
Go to: https://app.roboflow.com

### Step 2: Create an Account or Log In
You may sign up using:
- Google account
- GitHub
- Email address

# PART 2: Creating a New Project
### Step 1: Click **Create New Project**
Fill in the following:
| Field | What to Enter |
|--------|--------------|
| Project Name | `Student_Lab_Roboflow` |
| Project Type | Object Detection |
| Annotation Group | Leave default |
| License | Public (for classroom use) |
Click **Create Public Project**

# PART 3: Define Labels (Classes)
After creating the project:
1. Click **Upload**
2. Upload your images (5–20 images minimum)
3. Click **Finish Uploading**
During annotation, you will define labels.

### Example Labels
| Label Name |
|------------|
| Class1 |
| Class2 |

For medical version:
- Pneumonia
- Normal

# PART 4: Annotating Images (Bounding Boxes)
After upload:
1. Click an image to start annotating
2. Click **Add Annotation**
3. Select **Bounding Box**
4. Draw a box around the object
5. Enter label name
6. Press **Enter** or click **Save**
Repeat for all objects in the image.

# Navigating Between Images
- Use **Next Image** button  
- Click image thumbnails from dataset list  
- Use zoom tool for better accuracy  

# Annotation Best Practices
✔ Draw tight bounding boxes  
✔ Be consistent across images  
✔ Label all visible objects  
✔ Avoid overlapping incorrect labels  

# BEGINNER LAB ACTIVITY

# Lab Title: Basic Object Detection Annotation Using Roboflow
## Objective
Annotate a small dataset and export it in YOLO format for model training.

## Dataset Requirement
Download or prepare:
- 10–20 images containing at least 2 object types  
  (Example: Cats & Dogs OR Medical: Normal & Pneumonia X-rays)

# Step-by-Step Laboratory Procedure
## Step 1: Login to Roboflow
Go to: https://app.roboflow.com

## Step 2: Create New Project
- Project Name: `Lab1_ObjectDetection`
- Project Type: Object Detection
- Click **Create**

## Step 3: Upload Dataset
1. Click **Upload**
2. Drag and drop images
3. Click **Finish Uploading**

## Step 4: Annotate All Images
For each image:
1. Click image  
2. Select **Bounding Box Tool**  
3. Draw box around object  
4. Assign correct label  
5. Save  
6. Move to next image  
Repeat until all images are labeled.

## Step 5: Generate Dataset Version
1. Click **Generate**
2. Choose preprocessing (leave default for beginners)
3. Click **Generate Version**

## Step 6: Export Dataset
1. Open the generated version
2. Click **Download Dataset**
3. Select format:
   - YOLOv5
   - YOLOv8
   - COCO
4. Download ZIP file

# Optional Medical Informatics Version
For health analytics adaptation:
### Labels:
- Pneumonia
- Normal
Students can:
- Annotate chest X-rays
- Generate dataset version
- Export in COCO format
- Use dataset for CNN or YOLO training
