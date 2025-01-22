# AqUavplant Dataset: Aquatic Plant Classification and Segmentation High Resolution UAV Image Dataset
AqUavplant Dataset: An Aquatic Plant Classification and Segmentation High-Resolution Image Dataset using Unmanned Aerial Vehicle RGB Camera. This repository is for custom data loader and benchmarking all the baselines in PyTorch.
This work is the benchmarking code for the AqUavplant dataset. The article is accepted in Scientific Data, Nature journal and is titled 'AqUavplant Dataset: A High-Resolution Aquatic Plant Classification and Segmentation Image Dataset Using UAV'. The full paper link: https://www.nature.com/articles/s41597-024-04155-6

# Dataset Annotation
The dataset has been annotated using Fiji and details of the process is given [here](https://github.com/aia39/Multiclass-Semantic-Segmentation-Annotation-tool-usage-codes).

# Dataset download
The dataset will be available upon article publication. It is uploaded publicly in figshare. Link: https://figshare.com/articles/dataset/AqUavplant_Dataset_A_High-Resolution_Aquatic_Plant_Classification_and_Segmentation_Image_Dataset_Using_UAV/27019894

# Dataset organization

The dataset is organized based on the type of split. So the user can organize the codes accordingly.

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

# Citation 
```BibTeX
@article{istiak2024aquavplant,
  title={AqUavplant Dataset: A High-Resolution Aquatic Plant Classification and Segmentation Image Dataset Using UAV},
  author={Istiak, Md Abrar and Khan, Razib Hayat and Rony, Jahid Hasan and Syeed, MM Mahbubul and Ashrafuzzaman, M and Karim, Md Rajaul and Hossain, Md Shakhawat and Uddin, Mohammad Faisal},
  journal={Scientific Data},
  volume={11},
  number={1},
  pages={1411},
  year={2024},
  publisher={Nature Publishing Group UK London}
}
```

