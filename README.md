# AqUavplant Dataset: Aquatic Plant Classification and Segmentation High Resolution UAV Image Dataset
AqUavplant Dataset: An Aquatic Plant Classification and Segmentation High-Resolution Image Dataset using Unmanned Aerial Vehicle RGB Camera. This repository is for custom data loader and benchmarking all the baselines in PyTorch.
This work is the benchmarking code for the AqUavplant dataset. The article is submitted to a journal and it is titled as 'AqUavplant Dataset: A High-Resolution Aquatic Plant Classification and Segmentation Image Dataset Using UAV'

# Dataset download
The dataset will be available upon article publication. It is uploaded privately in figshare.

# Dataset organization

The dataset is organized based on the type of split. So, user can organize accordingly to run the codes: 
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


classwise_split/
   train/
      ...
   validation/
      ...
   test/
      ...

```

# Installation
   ```bash
   pip install -r requirements.txt
   ``` 
N.B: Install pytorch-gpu from conda if it mismatches.

# Running codes
* For binary semantic segmentation run the notebook 'AqUavplant-binary-segmentation.ipynb'. There are five models in the notebook, one can be used by uncommenting the corresponding block. After running the whole code, all the output results and figures will be saved.
* For multiclass semantic segmentation run the notebook 'aqUavplant-multiclass-segmentation.ipynb'. There are five models in the notebook similar to binary one, one can be used by uncommenting the corresponding block.
* Also, some newer models i.e., Swin transformer and Deeplabv3 codes were uploaded.

# Models 
The models that are in the codes are:
1. U Net
2. R2Unet
3. Attention U Net
4. R2Attention U Net
5. DeepLabV3 (resnet 50, resnet101, mobilenet V3)
6. DeepLabV3 plus
7. Swin Transformer


# Acknowledgement
Thanks to the repository: https://github.com/LeeJunHyun/Image_Segmentation/tree/master, for his model architecture codes in pytorch.

