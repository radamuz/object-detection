# object-detection
## Info
* This code was not written by me from scratch, the real author is Moses Olafenwa.  

* The source where I got it is https://www.datasciencecentral.com/profiles/blogs/object-detection-with-10-lines-of-code

## Requirements
* Install python3
```bash
sudo apt install python3
```
* Install Pip (Python package manager)
```bash
sudo apt install python3-pip
```

* To run the code, you must install the following Pyton libraries, via pip
```bash
pip3 install Tensorflow testresources Numpy==1.19.3 SciPy==1.4.1 opencv-python Pillow Matplotlib==3.3.2 H5py Keras ImageAI
```

* Drivers needed to run this code on nvidia
```bash
sudo apt install -y --no-install-recommends nvidia-compute-utils-450 nvidia-dkms-450 nvidia-driver-450 nvidia-kernel-common-450 nvidia-kernel-source-450 nvidia-utils-450 libnvinfer7=7.1.3-1+cuda11.0 libnvinfer-dev=7.1.3-1+cuda11.0 libnvinfer-plugin7=7.1.3-1+cuda11.0
```


The following packages have unmet dependencies:
 nvidia-driver-450 : Depends: nvidia-dkms-450 (= 450.102.04-0ubuntu1)
                     Depends: nvidia-kernel-source-450 (= 450.102.04-0ubuntu1) but it is not going to be installed
                     Depends: libnvidia-compute-450 (= 450.102.04-0ubuntu1) but it is not going to be installed
                     Depends: libnvidia-extra-450 (= 450.102.04-0ubuntu1) but it is not going to be installed
                     Depends: nvidia-compute-utils-450 (= 450.102.04-0ubuntu1) but it is not going to be installed
                     Depends: libnvidia-decode-450 (= 450.102.04-0ubuntu1) but it is not going to be installed
                     Depends: libnvidia-encode-450 (= 450.102.04-0ubuntu1) but it is not going to be installed
                     Depends: nvidia-utils-450 (= 450.102.04-0ubuntu1) but it is not going to be installed

git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch resnet50_coco_best_v2.0.1.h5" \
  --prune-empty --tag-name-filter cat -- --all
git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch nvidia-machine-learning-repo-ubuntu1804_1.0.0-1_amd64.deb" \
  --prune-empty --tag-name-filter cat -- --all


## Information sources
* <https://github.com/tensorflow/tensorflow/issues/45930>
* Solve problems with nvidia graphics: 
  * <https://www.tensorflow.org/install/gpu#install_cuda_with_apt>
* <https://stackoverflow.com/questions/5226311/installing-specific-package-versions-with-pip>
* Download the RetinaNet model file that will be used for object detection:
  * <https://github.com/OlafenwaMoses/ImageAI/releases/download/1.0/resnet50_coco_best_v2.0.1.h5>
* <>
