# Separated, Cross-Fused and Extensible G&L Fusion Network for LiDAR Semantic Segmentation
### State Key Lab of Rail Traffic Control & Safety (BJTU)
This repo contains the source code and dataset for our paper:
<br>
[**Separated, Cross-Fused and Extensible G&L Fusion Network for LiDAR Semantic Segmentation**](https://github.com/mapping520/SAMe3d/)
<br>
[paper](https://github.com/mapping520/SAMe3d/)
![SAMe3d](/Figs/Backbone_work.Png)


# Step1.Environment Installation
our paltform configuration: ubuntu18.04, Nvidia RTX 3090, cuda11.4, python3.7(in anaconda environment).
note: we didn't testing in other configuration.

## Requirements

Ensure that the installation of the GPU driver(cuda,cudnn) is **completed** before the belows.


- Create a virtual environment and activate it.(optional)
```
conda create -n SAMe3d python=3.7
conda activate SAMe3d
```
- PyTorch >= 1.2(optional)
```
conda install pytorch torchvision torchaudio
```
