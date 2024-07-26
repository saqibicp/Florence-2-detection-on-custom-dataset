# **Florence 2 Detection on Custom Dataset:**
This project demonstrates how to use Florence 2 for object detection on a custom dataset. The dataset annotations are converted from YOLO format to the Florence-2 suitable format.
## **Florence 2 Overview:**
Florence-2 is a cutting-edge vision model that handles various tasks, including captioning, object detection, and segmentation, through a prompt-based approach. Trained on the extensive FLD-5B dataset with 5.4 billion annotations across 126 million images, it excels in multi-task learning. Its sequence-to-sequence architecture allows it to perform well in both zero-shot and fine-tuned scenarios, making it a leading vision foundation model.
### **Requirements:**
Install the required dependencies by running:

pip install -r requirements.txt

or by executing the first cell of the Florence_2_detection_custom_dataset.ipynb file.
### **Data Preparation**:
Prepare your data in a format suitable for the Florence 2 model: {

    "image": "image_name.jpg",
    
    "prefix": "<OD>",
    
    "suffix": "<loc_x1><loc_y1><loc_x2><loc_y2>...<loc_xN><loc_yN>"}
if labels are in YOLO format then change it to Florence-2 suitable form using "florence2_json_label_preparation.ipynb" 
## **Training:**
To train Florence 2 on your custom dataset, run the Florence_2_detection_custom_dataset.ipynb file.
