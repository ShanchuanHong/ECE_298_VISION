# Waste Detection and Classification Using Machine Learning Models

**Members:** Shanchuan Hong, Kezhou Chen

## 1. Problem Statement
Globally, environmental pollution from improperly managed waste in natural settings is intensifying. This waste not only undermines the aesthetic appeal of landscapes but also poses severe threats to wildlife and ecosystems. Developing an efficient and accurate system for identifying and classifying waste is crucial for effective pollution management.

## 2. Background
The growing urgency to mitigate waste pollution has spurred the exploration of technology-driven solutions. Advanced object detection models, utilizing image recognition technology, have demonstrated significant potential across various domains. This project aims to leverage the latest advancements in machine learning to address the challenges of waste detection in natural environments, thereby enhancing waste management processes to be more efficient and less labor-intensive.

## 3. Methodology
### Model Overview
- **YOLO (You Only Look Once)**: A leading model in object detection, YOLO is celebrated for its fast processing speeds, making it ideal for real-time applications. It detects objects by predicting bounding boxes and class probabilities simultaneously.
  - **YOLOv5**: Among the YOLO versions, we are considering YOLOv5 primarily because of its optimal balance between speed and accuracy, which could be ideal given the constraints of our available hardware. YOLOv5 has shown significant improvements in both performance metrics and efficiency over its predecessors, making it a strong candidate for our needs.

### Alternative Models
- **Detectron2**: Developed by Facebook AI Research, Detectron2 is built using PyTorch and is known for its flexibility and efficiency in implementing and training object detection algorithms. It supports various architectures including Faster R-CNN, which is famous for its high accuracy.
- **Faster R-CNN**: Known for its precision, Faster R-CNN effectively separates detection into region proposal and object classification, making it ideal for scenarios where detail is paramount.

### Tasks
- **Data Preprocessing**: Convert the TACO dataset or other suitable datasets into the COCO format to standardize inputs across models, facilitating the integration of pre-trained models.
- **Model Finetuning**: Begin with a pre-trained YOLOv5 model and fine-tune it using our specific dataset to enhance model generalization and detection accuracy.
- **Model Evaluation**: Assess alternative models like Detectron2 and Faster R-CNN alongside YOLOv5 to determine the optimal solution based on accuracy, processing speed, and computational efficiency.

## 4. Dataset
This project will utilize several datasets, each providing unique insights and contributions to our model training and validation processes:
- **TACO (Trash Annotations in Context) Dataset**: A comprehensive dataset designed for the classification and detection of litter in varied environments, featuring thousands of manually annotated images from settings like beaches, urban areas, and parks.
- **Trash-ICRA19 Dataset**: Developed for the IEEE ICRA 2019 conference, this dataset includes images of underwater waste, complementing TACO with scenarios not typically covered, and enhancing model robustness in diverse environments.
- **Cigarette Butt Dataset**: Specifically curated to detect cigarette butts, this dataset targets one of the most common forms of litter, providing focused data that enhances detection in realistic scenarios.
