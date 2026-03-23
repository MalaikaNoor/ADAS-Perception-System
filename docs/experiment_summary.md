# Experiment Summary

This project evaluates deep learning models for perception tasks in Advanced Driver Assistance Systems (ADAS), focusing on object detection and semantic segmentation using real-world urban driving scenes.

## YOLOv7 Object Detection

The YOLOv7 model was applied to multiple road scene images to detect dynamic objects such as vehicles and pedestrians. The model demonstrated strong detection performance, particularly for large and clearly visible objects. Bounding box predictions were generally accurate and well-localised.

However, some limitations were observed. Detection performance decreased for smaller or distant objects, and in scenes with higher complexity (e.g., dense traffic), some objects were missed or detected with lower confidence. Despite this, YOLOv7 maintained fast inference and is well suited for real-time ADAS applications.

## SegFormer Semantic Segmentation

SegFormer was used to perform semantic segmentation and provide pixel-level understanding of the driving environment. The model successfully identified key scene components such as roads, sidewalks, and surrounding infrastructure.

The segmentation outputs provided important contextual information that is not available through object detection alone. For example, the model clearly distinguished drivable areas from non-drivable regions. However, some boundary regions (e.g., between road and sidewalk) were less precise, indicating limitations in fine-grained segmentation.

## Combined Perception Insight

The experiments highlight the complementary strengths of object detection and semantic segmentation. YOLOv7 provides instance-level information by identifying specific objects, while SegFormer provides global scene understanding through pixel-level classification.

By combining both approaches, a more complete representation of the driving environment can be achieved. This integration is important for ADAS systems, where both object awareness and contextual understanding are required for safe decision-making.

## Key Observations

- YOLOv7 performs well for real-time object detection but struggles with small or distant objects
- SegFormer provides strong contextual understanding but lacks instance-level detection
- Combining detection and segmentation improves overall perception capability
- Model performance can vary depending on scene complexity and environmental conditions

## Conclusion

Overall, the experiments demonstrate that combining efficient object detection models with semantic segmentation models provides a practical and effective approach for ADAS perception systems. The results support the design of the proposed perception pipeline and highlight the importance of balancing accuracy, computational efficiency, and real-time performance.
