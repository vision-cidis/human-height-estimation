Before starting to use this project,  there are some requirements to fullfill.

## Requirements
* [Python 3.7.3](https://www.python.org/downloads/release/python-370/g)
  
Once the packages are installed,  clone this repo as follow: 

    git clone https://github.com/vision-cidis/human-height-estimation.git

# Deep Learning-based Human Height Estimation from a Stereo Vision System
This paper presents a deep learning-based human height estimation approach using a stereo vision system, which is part of a smart receptionist framework. The proposal consists of a smart screen with an integrated webcam and an additional webcam. The workflow of this approach initially acquires and processes the images in real-time, using deep neural networks detects a human in the images, aligns the images from the two cameras, then obtains the depth of the camera, and finally computes the height of the person under study. The proposed solution is evaluated by different people to check the effectiveness of the system. Obtained results show MAE below 1.0 cm in the computed heights, it is also compared with other techniques of the state-of-the-art.

# Citation
Please cite those paper if you find helpful,
```
@inproceedings{velesaca2023deep,
  title={Deep Learning-based Human Height Estimation from a Stereo Vision System},
  author={Velesaca, Henry O and Vulgarin, Jorge and Vintimilla, Boris X},
  booktitle={2023 IEEE 13th International Conference on Pattern Recognition Systems (ICPRS)},
  pages={1--7},
  year={2023},
  organization={IEEE}
}
```
