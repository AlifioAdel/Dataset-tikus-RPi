# Training and Testing dataset model with YoloV8n base model for Mouse/Rat detection

## Dataset Model
Terdapat 4 dataset model yang digunakan dalam training dan testing model ini, yaitu:
1. MouseDetec Dataset [Roboflow](https://universe.roboflow.com/shaun-liew-ogtx2/mouse-detection-51iyt/dataset/1)
2. MouseV2 Dataset [Roboflow](ttps://universe.roboflow.com/mouse-dataset/mouse-v5ogi/dataset/2)
3. PiMouse Dataset [Roboflow](https://universe.roboflow.com/yuan-swpfw/piratcy-object-detection/dataset/2)
4. TryMouse Dataset [Roboflow](https://universe.roboflow.com/ttt-lq7ks/testforme/dataset/1)

## Base Model
Base model yang digunakan dalam training model ini adalah model yolov8n.pt dari Ultralytics.

## Hasil dari Training Model
Model yang dihasilkan dari training ini dapat dilihat pada [folder runs](runs/detect/).
| Dataset | mAP50 | Precision | Recall | Train |
| --- | --- | --- | --- | --- | 
|MouseDetec | 0.908 | 0.894 | 0.856 | 4 |
|MouseV2 | 0.941 | 0.903 | 0.916 | 1 |
|PiMouse | 0.956 | 0.959 | 0.889 | 2 |
|TryMouse | 0.898 | 0.814 | 0.877 | 3 |

:exclamation: **Note**:
Dalam folder runs/detect/predict(1-4) merupakan hasil deteksi dari MouseV2 dan PiMouse dataset, yang berisi gambar dan video percobaan deteksi.

## Model
1. Dataset MouseV2
    - [pt file](runs/detect/train/weights/best.pt)
    - [onnx file](runs/detect/train/weights/best.onnx)
    - [tf file](runs/detect/train/weights/best_saved_model/best_float32.tflite)

2. Dataset PiMouse
    - [pt file](runs/detect/train2/weights/best.pt)
    - [onnx file](runs/detect/train2/weights/best.onnx)
    - [tf file](runs/detect/train2/weights/best_saved_model/best_float32.tflite)

3. Dataset TryMouse
    - [pt file](runs/detect/train3/weights/best.pt)
    - [onnx file](runs/detect/train3/weights/best.onnx)
    - [tf file](runs/detect/train3/weights/best_saved_model/best_float32.tflite)

4. Dataset MouseDetec
    - [pt file](runs/detect/train4/weights/best.pt)
    - [onnx file](runs/detect/train4/weights/best.onnx)
    - [tf file](runs/detect/train4/weights/best_saved_model/best_float32.tflite)