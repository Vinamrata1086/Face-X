# Overview

## *LBPH -> Local Binary Patterns Histogram*

It is based on local binary operator. It is widely used in facial recognition due to its computational simplicity and discriminative power. 

**It is very efficient texture operator which labels the pixels of an image by thresholding the neighborhood of each pixel and considers the result as a binary number.**
The steps involved to achieve this are:

* creating dataset
* face acquisition
* feature extraction
* classification

The LBPH algorithm is a part of opencv.


# Dependencies

    pip install numpy
    pip install opencv-python
    pip install skimage
# Images

<p align="center"><img src="https://github.com/Vinamrata1086/Face-X/blob/master/Recognition-Algorithms/Facial%20Recognition%20using%20LBPH/images/pic1.png"><br>
Divide face images into R( for example R = 3 x 3 = 9 Regions) local regions to extract LBP histograms.</p>


<p align="center"><img src="https://github.com/Vinamrata1086/Face-X/blob/master/Recognition-Algorithms/Facial%20Recognition%20using%20LBPH/images/pic2.png" ><br>
Three neighborhood examples used to define a texture and calculate a local binary pattern (LBP).</p>

<p align="center">
    <img src="https://github.com/Vinamrata1086/Face-X/blob/master/Recognition-Algorithms/Facial%20Recognition%20using%20LBPH/images/pic3.png"><br>
    After applying the LBP operation we extract the histograms of each image based on the number of grids (X and Y) passed by parameter. After extracting the histogram of each region, we concatenate all histograms and create a new one which will be used to represent the image.
</p>
    
# Quick-Start

- Fork the repository
>click on the uppermost button <img src="https://github.com/Vinamrata1086/Face-X/blob/master/Recognition-Algorithms/Facial%20Recognition%20using%20LBPH/images/fork.png" width=50>

- Clone the repository using-
```
git clone https://github.com/akshitagupta15june/Face-X.git
```
- Create virtual environment-
```
- `python -m venv env`
- `source env/bin/activate` (Linux)
- `env\Scripts\activate` (Windows)
```
- Install dependencies-

- Headover to Project Directory- 
```
cd Facial Recognition using LBPH

```
- Execute -
```
python facial_recognition_part1.py (face images collection)
python facial_recognition_part2.py (training)
python facial_recognition_part3.py (final recognition)
```
Note: Make sure you have haarcascade_frontalface_default.xml file 
