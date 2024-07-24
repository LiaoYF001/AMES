
# AMES: Adaptive Multi-modal Image Matching

Welcome to **AMES**, a highly adaptive multi-modal image matching project that leverages tuning-free filtering and enhanced sketch features.

## Data Structure

Data can be download at https://github.com/LiaoYF001/AMES/releases

The data is organized as follows:

```
DATA:
├── GF3
│   ├── 1
│   │   ├── pair1.tif
│   │   └── pair2.tif
│   ├── 2
│   │   ├── pair1.tif
│   │   └── pair2.tif
│   └── ...
├── GF7
│   ├── 1
│   │   ├── pair1.tif
│   │   └── pair2.tif
│   ├── 2
│   │   ├── pair1.tif
│   │   └── pair2.tif
│   └── ...
├── HJ2
│   ├── 1
│   │   ├── render
│   │   ├── pair1.tif
│   │   └── pair2.tif
│   ├── 2
│   │   ├── render
│   │   ├── pair1.tif
│   │   └── pair2.tif
│   └── ...
```

## Running the Demo

To run the demo, follow these steps:

1. **Install Matlab Runtime 9.13**:  
   Ensure you have Matlab Runtime 9.13 installed on your system.

2. **Place the `config.json` File**:  
   Put the `config.json` file in the same directory as `AMES_MAIN.exe`.

3. **Modify the `config.json` File**:  
   Adjust the `Folder` value in `config.json` to reflect the actual parent directory of the `DATA` folder (excluding `DATA`).

4. **Run `AMES_MAIN.exe`**:  
   Execute `AMES_MAIN.exe`. It is process-safe and supports concurrent multi-process execution for enhanced speed.

## Matching Your Own Data

To match your own data, follow these guidelines:

1. **Modify the Category**:  
   Adjust the `Category` value to include images from other categories.

2. **Set MaxIDs**:  
   Ensure the maximum ID number of folders under each category does not exceed the `MaxIDs` in `config.json`.

3. **Image Naming and Format**:  
   Name the image files as "pair1" and "pair2" with extensions ".tif", ".jpg", ".bmp", or ".png".

4. **Parameter Settings**:  
   You can modify the parameters in `config.json` as needed:
   - **Transform**: Can be "similarity", "affine", or "perspective".
   - **Border**: Can be 1 or 0, representing whether or not to force extraction of feature points close to the image boundary.
   - **ParaSet**: Can be "auto", "1", "2", "3", or "4", representing different parameter modes.

## Citation

If you find this project useful, please consider citing our paper:

Yifan Liao, Pengjie Tao, Qi Chen, Lei Wang, Tao Ke,  
"Highly adaptive multi-modal image matching based on tuning-free filtering and enhanced sketch features,"  
*Information Fusion*, 2024, 102599.  
ISSN 1566-2535, [https://doi.org/10.1016/j.inffus.2024.102599](https://doi.org/10.1016/j.inffus.2024.102599).
