***Quantification of Occlusion Handling Capability of a 3D Human Pose Estimation Framework (IEEE Transaction on Multimedia , 2022)***

This project is an implementation of paper: https://ieeexplore.ieee.org/document/9732169 ,

Video Demo of our work: https://www.youtube.com/watch?v=Y-R2bJ4zXME 


https://user-images.githubusercontent.com/53044443/168065063-f7e16d4a-4879-4458-8c2a-63680bcd9253.mp4



https://user-images.githubusercontent.com/53044443/168065129-4d458e35-361c-4876-bbbb-cd95990e4116.mp4


**Results on Human 3.6M**

![res_h36m](https://user-images.githubusercontent.com/53044443/168068179-d9176ff4-5d3a-476d-8a4b-e3152c699d86.png)



**Results on Action Classification on NTU-RGB+D (predictions from T3D-CNN)**


![res_action](https://user-images.githubusercontent.com/53044443/168068377-fa605e76-2e34-48ab-a978-7ee9f448f1a0.png)


**Dataset:**

The source code is for training/evaluating on the Human3.6M dataset. Our code is compatible with the dataset setup introduced by [Pavllo et al.](https://openaccess.thecvf.com/content_CVPR_2019/papers/Pavllo_3D_Human_Pose_Estimation_in_Video_With_Temporal_Convolutions_and_CVPR_2019_paper.pdf) Please refer to [VideoPose3D](https://github.com/facebookresearch/VideoPose3D )to set up the Human3.6M dataset (./data directory).


**Evaluate Pre-trained Model:**

In order to evaluate our pre-trained: [Pre-trainedModel](https://drive.google.com/drive/folders/1gHfyf6ufbVW2nh-9kS5mmUNSy8KN_bPb?usp=sharing )

Run:

```bash
python3 run_occ.py -k gt -arc 3,3,3,3,3 -c checkpoint --evaluate epoch_16Miss.bin 
```

**Train from Scratch:**

```bash
python3 run_occ.py -k gt -arc 3,3,3,3,3 -c checkpoint
```

**Bibtex**

If you use our code in your research. Please cite our paper:
```bash
@article{ghafoor2022quantification,
  title={Quantification of Occlusion Handling Capability of 3D Human Pose Estimation Framework},
  author={Ghafoor, Mehwish and Mahmood, Arif},
  journal={IEEE Transactions on Multimedia},
  year={2022},
  publisher={IEEE}
  }
  ```
  **Visualization:**

We keep our code consistent with VideoPose3D.
