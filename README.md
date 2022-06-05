# Faster-RCNN-Final-Project
Faster RCNN using three training approaches

# 训练步骤
数据集准备 本文使用VOC2007数据，训练开始前需下载好VOC2007 数据集并解压在根目录。

在VOC2007数据集上训练Faster RCNN，并使用Resnet-50作为backbone，使用以下三种方法：
1.随机初始化网络参数
2.ImageNet预训练backbone网络
3.使用coco训练的Mask R-CNN的backbone网络参数，初始化Faster R-CNN的backbone网络

在终端分别输入以下命令进行不同方式的训练
```
python train.py random
python train.py imagenet
python train.py coco
```
# 测试步骤
在detec.py 文件中修改对应图片和模型的路径，之后运行detect.py
