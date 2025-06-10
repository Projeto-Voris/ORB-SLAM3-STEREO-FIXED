# ORB-SLAM3-STEREO-FIXED

This repository is a modified version of [ORB_SLAM3](https://github.com/UZ-SLAMLab/ORB_SLAM3)  

--- 

## Modification
- Succesfully tested in **Ubuntu 22.04** and **ROS2 Humble**(with OpenCV 4.5.4)
- Update from C++11 to C++14
- Fixed unexpected <span style="color:red">error</span> when start **STEREO** mode with **Rectified** camera type  

## How to build
Clone the repository:
```
git clone https://github.com/Projeto-Voris/ORB-SLAM3-STEREO-FIXED.git ORB_SLAM3
```

Install {Pangloin](https://github.com/stevenlovegrove/Pangolin) on version 0.9.2
```
# Clone Pangolin along with it's submodules
cd ORB_SLAM3/Thirdparty
git clone --recursive -b v0.9.2https://github.com/stevenlovegrove/Pangolin.git
cd Pangolin
# Install dependencies (as described above, or your preferred method)
./scripts/install_prerequisites.sh recommended

# Configure and build
cmake -B build
cmake --build build
```
Execute:
```
cd ORB_SLAM3
chmod +x build.sh
./build.sh
```
This will create **libORB_SLAM3.so**  at *lib* folder and the executables in *Examples* folder.
