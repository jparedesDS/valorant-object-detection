# Valorant Players Detector

#### Supported Labels
['Body', 'Head']
- Model YOLOv10b: https://huggingface.co/jparedesDS/valorant-yolov10b

#### ALL my models YOLOv10 & YOLOv9 for Counter Strike 2
- Yolov9c: https://huggingface.co/jparedesDS/cs2-yolov9c
- Yolov10s: https://huggingface.co/jparedesDS/cs2-yolov10s
- Yolov10m: https://huggingface.co/jparedesDS/cs2-yolov10m
- Yolov10b: https://huggingface.co/jparedesDS/cs2-yolov10b

#### How to use
```
from ultralytics import YOLO

# Load a pretrained YOLO model
model = YOLO(r'weights\yolov10b_vlr.pt')

# Run inference on 'image.png' with arguments
model.predict(
    'image.png',
    save=True,
    device=0
    )
```
#### Confusion matrix normalized
![confusion_matrix_normalized.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/_yp5HjaiN54WjIur4HS8T.png)
#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/MtFhhrP7_kp4d2pJRC8ss.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/JLy3fffqvxIoY4C0wcwjR.png)
#### Predict
![train_batch34921.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/R0xOHQsHqSpq-8Hc8umRY.jpeg)
![val_batch0_pred.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/KWygqgi-Gka7eNdKCkPN1.jpeg)
```
YOLOv10b summary (fused): 383 layers, 20,414,236 parameters, 0 gradients, 97.9 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 36/36 [00:06<00:00,  5.30it/s]
                   all        999       2016      0.959      0.886      0.925      0.631
                  Body        966       1029      0.969      0.914      0.955       0.76
                  Head        936        987      0.948      0.857      0.896      0.503
```

#### Others models Counter Strike 2 YOLOv10m Object Detection
https://huggingface.co/jparedesDS/cs2-yolov10m
