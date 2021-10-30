# Skeleton-based Action Recogntion using Spatial Temporal Graph Convolutional Networks on the UCF-101 and HMDB benchmarks


This is the project repository for the research study *Skeleton-based Action Recogntion using Spatial Temporal Graph Convolutional Networks on the UCF-101 and HMDB benchmarks* presented by [Motasem S. Alsawadi](https://www.ucl.ac.uk/iccs/motasem-alsawadi) and [Miguel Rio](https://www.ucl.ac.uk/iccs/prof-miguel-rio).

[[arXiv]](https://arxiv.org/abs/2108.01309)

<p align="center">
<img src="https://user-images.githubusercontent.com/52717252/139516602-798e6cff-2c29-4719-ba2f-44dbfc5ebd1a.gif"
</p>
<p align="center">
Skeleton extraction from a UCF-101 sample
</p>

## Contents
* [1. Download UCF-101 skeleton dataset](https://github.com/malswadi/skeleton_ucf_hmdb#1-download-ucf-101-skeleton-dataset)
* [2. Download HMDB skeleton dataset](https://github.com/malswadi/skeleton_ucf_hmdb#2-download-hmdb-skeleton-dataset)
* [3. Storage info](https://github.com/malswadi/skeleton_ucf_hmdb#3-storage-info)
* [Citation](https://github.com/malswadi/skeleton_ucf_hmdb#citation)
* [Acknowledgements](https://github.com/malswadi/skeleton_ucf_hmdb#acknowledgements)

## 1. Download UCF-101 skeleton dataset

The [UCF-101](https://www.crcv.ucf.edu/data/UCF101.php) dataset provides a total of 13,320 clips classified into 101 action classes. The skeleton output layout has been extracting using the [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) system. Due to the variability of the duration of each clip, a fixed duration of 300 frames has been proposed. Therefore, if any video clip has less than 300 frames, we repeat the initial frames until reach the amount needed. Otherwise, if the video clip exceeds the frame number, we trim it. As a consequence, the spatio-temporal information of the skeleton of each video sample can be represented as a tensor with shape (18, 3, 300). An independent JSON file has been exported for each video sample. Thus, the outcome of this process are 13,320 JSON files with the skeleton information of the UCF-101 dataset. respectively. The UCF-101 skeleton dataset can be downloaded [here](https://drive.google.com/file/d/1no8xPvNnthycI0zcRcn0tZO-agairoC7/view).

## 2. Download HMDB skeleton dataset

The [HMDB](https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/) dataset provides a total of 6,766 video clips of 51 different classes. Similar to the UCF-101 skeleton dataset, the skeleton output layout has been extracting using the [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) system using the same fixed  length of 300 frames. Also, an independent JSON file has been exported for each video sample. Therefore, 6,766 JSON files with the skeleton information of the HMDB dataset. The HMDB skeleton dataset can be downloaded [here](https://drive.google.com/file/d/1no8xPvNnthycI0zcRcn0tZO-agairoC7/view).



## 3. Storage info

## Citation
If you are interseted to use this code for your research, please cite:

```
@article{Alsawadi2021,
author = {Alsawadi, Motasem S and Rio, Miguel},
journal = {arXiv preprint arXiv:2108.01309},
title = {{Skeleton Split Strategies for Spatial Temporal Graph Convolution Networks}},
year = {2021}
}
```

## Acknowledgements
The training code is written by [Motasem S. Alsawadi](https://www.ucl.ac.uk/iccs/motasem-alsawadi) and it is based upon the skeleton extraction guidelines provided  in *Spatial Temporal Graph Convolutional Networks for Skeleton-Based Action Recognition*, Sijie Yan, Yuanjun Xiong and Dahua Lin, AAAI 2018. [[Arxiv Preprint]](https://arxiv.org/abs/1801.07455)
