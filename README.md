# AqUavplant-Dataset-Aquatic-Plant-Classification-and-Segmentation-High-Resolution-UAV-Image-Dataset-
AqUavplant Dataset: An Aquatic Plant Classification and Segmentation High-Resolution Image Dataset using Unmanned Aerial Vehicle RGB Camera. This repository is for custom data loader and benchmarking all the baselines in PyTorch.
This work is the benchmarking code for AqUavplant dataset. The article is submitted to a journal and it is titled as 'AqUavplant Dataset: A High-Resolution Aquatic Plant Classification and Segmentation Image Dataset Using UAV'

# Dataset download
The dataset will be available upon article publication. It is uploaded privately in figshare.

# Dataset organization

Image directory tree:
```
locationwise_split/
   train/
      BAUbotanicalgarden/
         frame1/
            BAUbotanicalgarden_1_binary.png
            BAUbotanicalgarden_1_multiclass.png
            frame_1.jpg
         frame2/
            BAUbotanicalgarden_2_binary.png
            ....

      BAUmuseum/
         frame1/
            BAUmuseum_1_binary.png
            ....

   validation/
      Shaplabil1/
            Shaplabil1_1_binary.png
            ....

   test/
      Shaplabi2/
            Shaplabil2_1_binary.png
            ....


locationwise_split/
   train/
      ...
   validation/
      ...
   test/
      ...

```

# Running codes
* For binary semantic segmentation run the notebook 'AqUavplant-binary-segmentation.ipynb'. There are five models in the notebook, one can be used by uncommenting the corresponding block. Codes were run in kaggle. All the output results and figures will be saved after running the whole code.
* For multiclass semantic segmentation run the notebook 'aqUavplant-multiclass-segmentation.ipynb'. There are five models in the notebook similar to binary one, one can be used by uncommenting the corresponding block.

# Models 
The models that are in the codes are:
* U Net
* R2Unet
* Attention U Net
* R2Attention U Net
* DeepLabV3 (resnet 50, resnet101, mobilenet V3)

