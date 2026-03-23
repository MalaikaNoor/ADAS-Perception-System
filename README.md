# ADAS Perception System

This project investigates the design of a vision-based perception system for Advanced Driver Assistance Systems (ADAS) using deep learning techniques.

The system focuses on combining object detection and semantic segmentation to improve scene understanding in urban driving environments.

## Models Used

- YOLOv7 – real-time object detection
- YOLOX – alternative detection model for comparison
- SegFormer – semantic segmentation for scene understanding

## Experiments

Multiple experiments were conducted using real-world road scene images to evaluate model performance.

- YOLOv7 demonstrated strong real-time detection performance
- SegFormer provided detailed pixel-level segmentation of road environments
- YOLOX was tested as an alternative detection model for comparison

## Repository Structure
notebooks/ → experiment notebooks
results/ → model outputs (YOLOv7, SegFormer, YOLOX)
images/ → input test images
docs/ → experiment summary and notes

## Final Words

I implemented and evaluated multiple deep learning models for ADAS perception, including object detection and semantic segmentation. I conducted experiments on urban driving images, analysed qualitative results, and compared different architectures to understand their strengths and limitations.

## Notes

All experiments were conducted using pre-trained models and publicly available data. The focus of this project was on evaluating perception performance and understanding the trade-offs between accuracy, efficiency, and deployment feasibility.

## External Resources

The following open-source resources were used to support the implementation of the experiments:

- YOLOv7: https://github.com/WongKinYiu/yolov7  
- YOLOX: https://github.com/Megvii-BaseDetection/YOLOX  
- Hugging Face Transformers (for SegFormer): https://github.com/huggingface/transformers  

YOLOv7 and YOLOX were used directly from their official repositories to perform object detection experiments. SegFormer was implemented using the Hugging Face Transformers library, which provides pre-trained models for semantic segmentation.

All experiments were executed, modified, and analysed independently as part of this project.
