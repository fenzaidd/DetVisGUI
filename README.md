# DetVisGUI

GUI for easily visualizing detection results .


![alt tag](./demo/demo1.png)

---

**Show Pascal VOC training results:** 

```
$ python DetVisGUI.py --format VOC --img_root data/VOCdevkit/VOC2007/JPEGImages --anno_root data/VOCdevkit/VOC2007/Annotations --txt data/VOCdevkit/VOC2007/ImageSets/Main/train.txt --det_file data/VOCdevkit/voc_train_results.pkl
```

**Show Pascal VOC test results(no groundtruth):** 

```
$ python DetVisGUI.py --format VOC --img_root data/VOCdevkit/VOC2007/JPEGImages --anno_root data/VOCdevkit/VOC2007/Annotations --txt data/VOCdevkit/VOC2007/ImageSets/Main/test.txt --det_file data/VOCdevkit/voc_test_results.pkl --no_gt
```

**Show COCO val results:** 

```
$ python DetVisGUI.py --format COCO --img_root data/COCO/val2017_small --anno_root data/COCO/instances_val2017_small.json --det_file data/COCO/coco_val_results.pkl 
```

**Show COCO test results (no groundtruth):** 

```
$ python DetVisGUI.py --format COCO --img_root data/COCO/test2017_small --anno_root data/COCO/image_info_test-dev2017_small.json --det_file data/COCO/coco_test_results.pkl --no_gt
```

---

## Hotkeys

|     KEY    | ACTION                                     |
|:----------:|:------------------------------------------:|
|    ↑  ↓    | Change Image.                              |
|    →  ←    | Change detection threshold.                |
|     s      | Save plot image in output folder.          |
|     q      | Colse this GUI.                            |

