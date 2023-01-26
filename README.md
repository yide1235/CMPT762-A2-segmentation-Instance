# Segmentation-Instance
In the .ipynb file, there is two way of doing segmentation, the first approach use a fast-rcnn detection model first, then do U-Net based segmentation on detected boxes. The second one is end-to-end mask rcnn segmentation. It shows in engineering, end-to-end straining ometimes shows better accuracy.

##First part, train a fast rcnn model with detectron:

![f9dd39f2ba17a37330b91f0f4364f84](https://user-images.githubusercontent.com/66981525/212870432-5404ce03-76d7-4cb2-891b-d3d4b0bfc30d.png)
![1dd6611e2ba10e9cc421fa2ff6099eb](https://user-images.githubusercontent.com/66981525/212870488-adbc697f-6452-4931-930a-c68cf2780c4b.png)
For some result of fast-rcnn result:
![1](https://user-images.githubusercontent.com/66981525/212870816-7f83ee41-d88b-455e-a18b-4c96faf426a3.png)
![2](https://user-images.githubusercontent.com/66981525/212870890-5118e47d-5914-4c64-a670-f506959006a0.png)
![3](https://user-images.githubusercontent.com/66981525/212870904-7aede4fb-a24d-4036-b036-ebcae6280a6b.png)

then I use nested U-net structure for segmentation. some model structure, loss and result:
![4](https://user-images.githubusercontent.com/66981525/212871217-ed42a09f-477b-4e6f-9f86-a7b9ab8941ba.png)
![919f04f33d6b83e4f0bdc8bc77beb48](https://user-images.githubusercontent.com/66981525/212871236-6b2bb93f-3322-45f7-a94c-68ca86e25ce7.png)
![fb68f2425168d533ddcda34e6314bdb](https://user-images.githubusercontent.com/66981525/212871265-18587dbc-2b3e-45c4-bbc3-0c29a436333a.png)
![ea92ec51f2813e7178d37f8751b56e1](https://user-images.githubusercontent.com/66981525/212871280-31e3d413-c8ab-4aa7-989b-491646e2ddea.png)
![90e2831c749ff819b98d36a71710e2f](https://user-images.githubusercontent.com/66981525/212871299-0e0c8349-9b86-43fe-999a-8903693f5233.png)

end of this not end-to-end training pipeline.

##Second part
use mask rcnn for segmentation
![264db410a4b40e4fbb67d0471b8c391](https://user-images.githubusercontent.com/66981525/212871698-65342d6b-8997-4ff2-a3c9-802926ebe1b3.png)
![a44c5f7f7c8456d4b6d59ec84e2bd30](https://user-images.githubusercontent.com/66981525/212871711-41b9294e-9866-4d33-a951-64e87afac3c7.png)

At the end, end-to-end training shows better training accuracy. This is already widely used in DL.

LS
