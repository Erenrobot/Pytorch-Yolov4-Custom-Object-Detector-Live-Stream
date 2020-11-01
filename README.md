# Pytorch-Yolov4-Custom-Object-Detector-Live-Stream
This programs allows to train and test custom objects.

Those programs based on https://github.com/Tianxiaomo/pytorch-YOLOv4 instructions

I made some enhancements on those programs.


How to use:
Firstly download zip file at https://github.com/Tianxiaomo/pytorch-YOLOv4. Then, copy and change these files which I included. After that, change code according to number of class, batch size and image size.

Sample train cmd commands for 416*416 image and 1 class:
python train.py -b 2 -s 1 -l 0.001 -g 0 -pretrained .yolov4.conv.137.pth -classes 1 -dir ./data -train_label_path data/train.txt -epochs 50

Sample test cmd commands for 416*416 image and 1 class:
python models.py 1 checkpoints/Yolov4_epoch205.pth test/testa.jpg 416 416 test/_classes.txt

