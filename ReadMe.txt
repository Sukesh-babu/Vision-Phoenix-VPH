#To train the model
python train.py --workers 8 --device 0 --batch-size 16 --epochs 1 --img 640 640  --data data/V7_VPH.yaml --hyp data/hyp.scratch.custom.yaml --cfg cfg/training/yolov7_VPH_P4.yaml --name VPH --weights weights/yolov7.pt


#To run inference on images/videos without count
python detect.py --weights best.pt --source images --classes 0



####VPH Module
Defined in modules/common.py

