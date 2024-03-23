# CW_M_Task1
## Face Mask Detection
Fine Tuning YOLOv7 to detect people weariing face masks. 
### Problems
1. Most models trained for face mask detection find it difficult to differetiate face masks and thick beards.
2. Confusion in models regarding face masks and veils( prominent in countries like India )
3. Ambiguity  of results in case of crowded images/ videos.

### Solutions 
Most of the above problems are found in models due to lack of a diverse dataset. o, a collective solution is to form a dataset which caters to these issues. 
Therefore, this model is trained on a self-created dataset whoich contains:
 1. Images of bearded men to help the model cope with the first problem.
 2. Images of women in veils and transparent face covers rather than masks.
 3. Images of large crowds with both masked and unmasked people.
 
To do justice to the dataset, yolov7 is used. But, at the same time, prevention of overfitting through augmentations and regularization is implemented.

### Dataset
https://universe.roboflow.com/pranav-gupta-eqnfm/face-mask-detection-56hot
