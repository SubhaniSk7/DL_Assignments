																			YOLOV3 OBJECT DETECTION:
1. For train the images should be in data/coco/images/train2014
2. For detection we should give test image path in command line.
3. The labels files should be in data/coco/labels/train2014
4. The animals.data should be in cfg/



Commands:
To train:
> python train.py --data cfg/animals.data --config cfg/yolov3_.cfg --weights yolov3.weights -r

To detect:
> python detect.py cfg/yolov3_.cfg yolov3.weights data/dog.jpg data/animals.names

To validate:
> python valid.py cfg/animals.data cfg/yolov3_.cfg yolov3.weights
