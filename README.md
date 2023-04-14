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
- numba, torchpack
```
conda install numba
pip install torchpack
```
- open3d
```
pip install open3d
```
- spconv (for cuda version)
```
pip install spconv-cu113
```
- torch_scatter
```
conda install pytorch-scatter -c pyg
```
- strictyaml
```
 pip install strictyaml
```
- nuscene-devkit
```
 pip install --no-dependencies nuscenes-devkit==1.1.1
```

# Step2.Data Download and Preparation
We have organized these three datasets. To evaluate/train point cloud, you will need to **download** the required datasets.

- Sany (ours) - [Baidu Drive](https://github.com/mapping520/SAMe3d/)
- nuScenes - [Baidu Drive](https://github.com/mapping520/SAMe3d/)
- SemanticKITTI - [Baidu Drive(access code: qaos)](https://pan.baidu.com/s/1LL2LItLEQpOt4HLWodTpWQ?pwd=qaos)

# Step3.Train & Validate

- To train on Sany dataset, run
```
 python train.py -source scannet -target modelnet
```
- To train on nuScenes dataset, run
```
 python train.py -source scannet -target modelnet
```
- To train on SemanticKITTI dataset, run
```
 python train.py -source scannet -target modelnet
```

## Acknowledgments
We thanks for the opensource codebases, [Cylinder3D](https://github.com/xinge008/Cylinder3D) and [spconv](https://github.com/traveller59/spconv)
