# Blood Cell Detection - YOLO5 and YOLO8 DeepLearning

### OVERVIEW
![image](https://github.com/user-attachments/assets/428cca80-a6d7-4dbb-87db-23a1ae3db4f1)

This pioneering investigation delves into the revolutionary domain of blood cell detection by leveraging state-of-the-art YOLO (You Only Look Once) models, specifically YOLOv5n, YOLOv5x, YOLOv8n, and YOLOv8x. Harnessing the capabilities of deep learning, our study leads the way in advancing the precision and efficiency of blood cell detection—an essential aspect of medical diagnostics. Significantly, YOLOv8n emerges as a formidable contender, exhibiting an unprecedented precision level of 87.3% and a meticulous ability to minimize false positives. Conversely, the YOLOv5x model, boasting an outstanding recall rate of 90.6%, excels in capturing a diverse array of true positives. Elevating our exploration further, YOLOv8x showcases exceptional spatial accuracy, achieving the highest Intersection over Union (IoU) at 0.588 and a Dice Coefficient of 0.654. These findings not only redefine the landscape of medical diagnostics but also hold the potential to significantly reduce manual workload through the pioneering integration of deep learning technologies.

### RESULT
![image](https://github.com/user-attachments/assets/22c77bd1-2bc2-4823-af2f-841a969bb21c)

In the comparative analysis of YOLO models for blood cell detection, YOLOv8n emerges as a robust performer, boasting the highest precision at 0.873 and demonstrating a meticulous ability to minimize false positives. Moreover, YOLO v8n excels in mean Average Precision (mAP) with both mAP50 and mAP95 scores, reaching 0.935 and 0.664, respectively. Its balanced F1-Score of 0.876 underscores its proficiency in harmonizing precision and recall. YOLOv8n is well-suited for applications where precision is paramount, as in medical diagnoses where false positives may result in unwarranted interventions.

In contrast, YOLOv5x showed itself with an impressive recall rate of 0.906, indicating its ability to capture mostly positives. With a commendable F1-Score of 0.877, YOLOv5x maintains a balance of both recall and precision, which makes it a perfect fit for applications where maximizing true positive results is crucial, even if it means accepting some false positive results. However, it is essential to note that YOLOv5x exhibits a slightly lower precision compared to YOLOv8n.

YOLOv8x distinguishes itself with the highest Intersection over Union (IoU) at 0.588 and the highest Dice Coefficient at 0.654. These metrics suggest superior spatial overlap between predicted and ground truth bounding boxes, indicating a strong capability for accurate localization. YOLOv8x is well-suited for applications where precise object localization and spatial accuracy are paramount.

In conclusion, the choice among YOLO models relies on the particular needs of the blood cell detection task. YOLOv8n proves optimal in situations where emphasis is placed on precision, YOLOv5x excels when maximizing recall is crucial, and YOLOv8x stands out in tasks where accurate localization and spatial precision are paramount. Considering these strengths and trade-offs is crucial in aligning the model choice with the specific needs of the application at hand.

We obtain several results from the training carried out on the dataset, such as train/cls_loss, and val/cls_loss. Cls_loss is represented as classification loss so training/cls_loss and validation/cls_loss show the variation in classification loss in the training dataset and validation dataset.

 ![image](https://github.com/user-attachments/assets/354b624b-cc37-4f7b-aa96-66ab8261ae22)

Fig.1: YOLOv8n train and validation classification loss

Figure 1 displays the classification loss outcomes for both the training and validation datasets on YOLOv8n. A decrease in training loss and validation loss shows that the model is learning and improving its performance on the training set. It can be seen that the training loss has decreased while the validation loss is quite stable and has not decreased significantly. This shows signs of overfitting as the model cannot generalize the data well.


![image](https://github.com/user-attachments/assets/de46fce1-5605-4767-802b-bfdd8ea97c3c)

Fig.2: YOLOv8x train and validation classification loss

Figure 2 displays the classification loss outcomes for both the training and validation datasets on YOLOv8x. It can be inferred that both training and validation loss graphs have a small decrease, so it can be said that the loss is quite stable. However, the model can be said to have signs of overfitting because the validation loss graph is above the training loss graph.


![image](https://github.com/user-attachments/assets/38c76172-99ec-47ff-98cf-d9ee89077d48)

Fig.3: YOLOv5n train and validation classification loss

Figure 3 displays the classification loss outcomes for both the training and validation datasets on YOLOv5n. The results show that training loss has decreased significantly while validation loss has a stable loss value, so the model can be considered to have signs of overfitting because it is too focused on training data and can not generalize validation data.


![image](https://github.com/user-attachments/assets/8de1fdc9-3d00-479f-9ff7-9f5db8c1b6dd)

Fig.4: YOLOv5x train and validation classification loss

Figure 4 shows the classification loss outcomes for both the training and validation datasets on YOLOv5x. The results show that the validation loss decreased significantly in the first few epochs but then had a stable loss while the training loss had a stable loss value. However, it can be said to have signs of overfitting because the validation loss graph is above the training loss graph.



