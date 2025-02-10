# AI Pipeline for Image Segmentation and Object Analysis

## Hosted Link
```bash
https://iona-pipe.streamlit.app/

```
## Project Overview

# AI-Driven Image Analysis Pipeline  

This project leverages deep learning to segment and recognize objects in images. It extracts and organizes segmented elements, generates descriptive captions, and presents insights through an interactive Streamlit web application.  

## Key Features  

- **Object Segmentation**: Utilizes Mask R-CNN for precise delineation of image components.  
- **Object Recognition**: Implements YOLO and Faster R-CNN for accurate classification.  
- **Caption Generation**: Produces contextual descriptions using CLIP.  
- **Data Management**: Stores object metadata efficiently with SQLite.  
- **User-Friendly Interface**: Provides real-time image processing via a Streamlit-powered web app.  






## Models and Tasks


### 1. Mask R-CNN (maskrcnn_resnet50_fpn)  
- **Function**: Object Segmentation  
- **Role**: Detects and isolates objects within an image, generating masks, bounding boxes, and classification labels.  

### 2. VGG16  
- **Function**: Object Recognition  
- **Role**: Classifies segmented objects with high accuracy using a pre-trained deep learning model.  

### 3. BLIP (Salesforce/blip-image-captioning-base)  
- **Function**: Captioning & Summarization  
- **Role**: Generates meaningful textual descriptions and summaries for identified objects.  

### 4. EasyOCR  
- **Function**: Text Detection & Extraction  
- **Role**: Identifies and extracts embedded text from segmented objects or images for further analysis.  


- **app.py**: The main application file integrating all steps of the pipeline and serving the Streamlit interface.
- **segmentation.py**: Contains the code for segmenting images using Mask R-CNN.
- **identification.py**: Handles object identification using pre-trained models.
- **mapping.py**: Maps identified objects to their descriptions.
- **data/**: Directory for storing input images, segmented objects, and the SQLite database.
- **requirements.txt**: Lists all dependencies required to run the project.

