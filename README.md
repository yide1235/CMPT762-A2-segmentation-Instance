# segmentation-instance
In the .ipynb file, there is two way of doing segmentation, the first approach use a fast-rcnn detection model first, then do U-Net based segmentation on detected boxes. The second one is end-to-end mask rcnn segmentation. It shows in engineering, end-to-end straining ometimes shows better accuracy.

First part, train a fast rcnn model with detectron:
![f9dd39f2ba17a37330b91f0f4364f84](https://user-images.githubusercontent.com/66981525/212870432-5404ce03-76d7-4cb2-891b-d3d4b0bfc30d.png)
![1dd6611e2ba10e9cc421fa2ff6099eb](https://user-images.githubusercontent.com/66981525/212870488-adbc697f-6452-4931-930a-c68cf2780c4b.png)
