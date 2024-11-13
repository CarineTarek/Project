# Project Idea
Dataset manipulation techniques is essential for extracting meaningful insights from data. It forms the foundation for accurate analysis, model building, and decision-making in various fields 


**Requirements**

The following Python libraries are required for this project:

* **OpenAI:** `openai==0.28`
* **Image Processing and Machine Learning:**
    * `torch`
    * `torchvision`
    * `transformers`
    * `opencv-python`
    * `matplotlib`
    * `numpy`
    * `timm`
    * `mmengine`
* **Inpainting Library:**
    * `simple-lama-inpainting==0.1.0`
* **Additional Libraries:**
    * `jupyter_bbox_widget`
    * `roboflow`
    * `dataclasses-json`
    * `supervision`
    * `ultralytics`
    * `diffusers`
    * `safetensors`
    * `accelerate`
    * `requests`

**Installation:**

To install these dependencies, use the following command:

pip install -r requirements.txt

**_Essential.py_** :The code snippet showcases a workflow that involves file handling, downloading resources, setting up a model for image captioning, and processing images and masks in specific directories. 
It provides a foundation for more advanced image processing and machine learning tasks, but completeness and successful execution would require resolving the missing imports and dependencies.

**_Packages.py_** : This file is a list of imports in the Python script covers a wide range of libraries and modules that are essential for various tasks, including data manipulation, image processing, machine learning, visualizationMake sure to import all

**_Dalle.py_** : In this file processing images using a YOLOv10 detection model, generating masks, and performing various image processing tasks based on these masks Also processes images in the temp_folder by converting black pixels to transparent pixels and saves the modified images in the output_folder. It iterates through all PNG and JPG files in the input folder, applies the transparency transformation

**_Removal.py_** : Python script that performs various image processing tasks, including converting JPEG images to PNG, running object detection using YOLOv10, generating masks, and saving processed images with bounding boxes and masks. Python code defines two functions, inpaint_with_lama.

**_Removal_only.py_** :This script provides a comprehensive image editing pipeline focused on removing or replacing elements within images. Also this script focuses on inpainting images using LaMa (Large Mask Inpainting with Differentiable Renderer) after object removal through masks.

# Usage 

_`dalle_init.py`_ : For processing images, converting image formats, performing object detection using YOLOv10, and handling masks and image segmentation tasks.

_`dalle_main.py`_:The code appears to be designed for automating the generation of prompts for DALL-E 2 image editing based on input images and masks. It processes images with various actions such as replacement, removal, and creation, providing a visual comparison between the original and edited images.

_`dalle_mask.py`_:This file contains functions are designed to batch process images in a folder, convert black pixels to transparency, and save the modified images in another specified output folder. The code provides a simple and effective way to make black pixels transparent in images.

_`dalle_gen.py`_: This is a file where we call all the functions we used in this files 

_`rem_rep_comb.py`_ : This code has function serves as an interface between the user's desired image edits and DALL-E 2's image generation capabilities. It takes in information about the image, the desired modifications, and generates a prompt that can be used to guide DALL-E 2 to produce the desired output.

_`rem_rep_init.py`_: This code provides a comprehensive pipeline for processing images, focusing on object detection, segmentation mask generation, and image manipulation

_`rem_rep_main.py`_:This code defines several functions for processing images using masks and generating captions with OpenAI API

_`rem_rep_process.py`_: This code defines functions for inpainting images with LaMa (Large Mask Inpainting with Differentiable Renderer) and provides functionalities for processing images in batches.

_`rem_rep_gen.py`_: This script appears to be a multi-step process for removing and replacing elements in images using a combination of techniques and tools. In this file We call all the function we created on this part of removal 

_`Removal_only.py`_: This code performs image editing with object removal and potentially segmentation functionalities It uses YOLOv10 for detection and a segmentation model (potentially Sam) to generate masks. It performs filtering, visualization, and data recording for processed images.

_`Removal_onlygen.py`_: This code where we can call all the function we build for see the output needed

_`Removal_onlymain.py`_: This code performs image inpainting, which fills in missing or unwanted regions in an image.


# License 
Project represented by Laila 




