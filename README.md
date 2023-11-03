A Rapid Screening Method for Suspected Defects in Steel Pipe Welds by Combining Correspondence Mechanism and Normalizing Flow

<img width="972" alt="方法图" src="https://github.com/aoihd/RSM/assets/141041853/431bc7ee-4c5d-4f04-85ff-6535eef80999">


![4](https://github.com/meiguiz/SISG-Net/assets/90629126/45422f9a-5495-4f1e-a03e-2c2958ed1b43)
![5](https://github.com/meiguiz/SISG-Net/assets/90629126/c43d4be2-edf5-42f9-b2f4-a39c3a27bf01)
![6](https://github.com/meiguiz/SISG-Net/assets/90629126/6dd35863-37a4-44ab-b742-08cf11dc7ffd)
![demo](https://github.com/aoihd/RSM/assets/141041853/3ddeb7cb-8319-4646-b8aa-fa7a6b14b6a7)
![微信图片_20231030230537](https://github.com/aoihd/RSM/assets/141041853/68b73612-ac09-4890-8a04-e9f39414e975)


The video of our experiment used in this paper can be found at: https://youtu.be/G_8USOwFXVs

The relabled OCID dataset can be found at: https://drive.google.com/file/d/1-XBstG9ur90E4X66gdG_OLVidCR56pgV/view?usp=drive_link


1. Setup anaconda environment
```
python=3.7
torch=1.9.0
cuda=11.1
```
2. Set the path to the dataset in config file.
### Train

1. Download the OCID dataset at https://drive.google.com/file/d/1-XBstG9ur90E4X66gdG_OLVidCR56pgV/view?usp=drive_link.
2. Unzip the downloaded dataset, and modify the `dataset_path` of the config file correspondingly.
3. To train an SISG-Net on OCID dataset. 
```
$ python train.py --gpu 0 --cfg rgb_depth
