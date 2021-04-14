# ROS Wrapper for DeepLab

This is the framework used in COEN490 Team 14 Tree-planting robot, terrain classification subsystem.

## Citing

If you use the code for your research, please cite this work as:
```bibtex
@misc{grinvald2018deeplabros,  
  author={Margarita Grinvald},
  title={ROS Wrapper for DeepLab},
  year={2018}
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/ethz-asl/deeplab_ros}},
}
```
<p align="center">
<img src="https://raw.githubusercontent.com/ethz-asl/deeplab_ros/master/doc/deeplab_ros.gif" width="600">
</p>

## Getting started
Clone this repository to the `src` folder of your catkin workspace, build your workspace and source it.

```bash
cd <catkin_ws>/src
git clone git@github.com:ethz-asl/deeplab_ros.git
catkin build
source <catkin_ws>/devel/setup.bash
```

## Example usage
An example launch file is included processing a sequence from the [Freiburg RGB-D SLAM Dataset](https://vision.in.tum.de/data/datasets/rgbd-dataset/download).

```bash
cd <catkin_ws>/src/deeplab_ros
chmod +x scripts/download_freiburg_rgbd_example_bag.sh 
scripts/download_freiburg_rgbd_example_bag.sh
roslaunch deeplab_ros freiburg.launch
```

