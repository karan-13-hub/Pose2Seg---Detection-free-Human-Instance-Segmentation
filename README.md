# Pose2Seg : Pose-based Human Instance Segmentation Framework

## The Detection Free Human Instance Segmentation pipeline is divided into : 
 - Affine-Align Operation
   - Pose Representation : There are 17 joints (as in COCO- our training dataset), each joint has 3 coordinates - (x,y,v) which are for position in image and visibility. So, each pose is represented by R 17x3 vector. Distance metric used for K-means is euclidean distance. We only consider poses with more than 8 valid points for K-means clustering. Mean vector of the class after clustering is taken as the representative element of the class (class template) which is used for pose detection in future
   - Pose Templates
   - Estimate Affine Transformation Matrix
 - Skeleton Features
 - SegModule

Download pretrained weights and resnet50 pytorch file from below link

https://drive.google.com/file/d/1D9MWWRKiWHyFE6Pm7busmX26oXLYW_Jx/view?usp=sharing
