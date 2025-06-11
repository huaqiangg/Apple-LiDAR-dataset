# Apple LiDAR Pavement Cracks Dataset

## Overview
This dataset contains pavement crack point clouds collected using Apple LiDAR on an iPad 21 Pro at Sun Yat-sen University, Zhuhai Campus. The dataset is intended for research on the potential application of Apple LiDAR in pavement crack detection.

## Data Collection Details
- **Device**: iPad 21 Pro or iPhone 16 Pro  
- **Software**: SiteScape  
- **Point Cloud Density**: Premium  or Medium
- **Point Cloud Size**: Small  
- **File Format**: .ply  
- **Each File Represents**: A single crack  

## Crack Measurement Attributes
- **Measurement Tool**: A vernier caliper with a resolution of **0.01mm** was used to measure crack width and depth.  
- **Crack Type Annotation**: Crack types (**transverse, longitudinal, alligator, and block cracks**) were manually labeled based on visual inspection.  
- **Measurement Variability**: Due to different crack characteristics, some width measurements represent average values.  
- **Weather Conditions**: Data was collected during **light rain**, and the point cloud may include water accumulation in cracks.  
- **Measurement Consistency**: All measurements were conducted by the **same team** to ensure consistency.  

## 📍 Crack Collection Locations
The image below shows the collection locations of different point cloud samples:

![Crack Collection Locations](crack.png)

## Dataset Download
The full dataset (~40GB) is available for download from an external source due to its large size.
| Crack ID | Crack Type | Density  | Crack Width | Crack Length | Crack Depth | Download Link |
|----------|------------|----------|-------------|--------------|-------------|---------------|
| sysu001  | Longitudinal | Premium | 4-14 mm     | 5.91 m  | 50-90 mm | [Download](#) |
| sysu002  | Transverse   | Premium | 4.4 mm      | 3.47 m | 10-50 mm | [Download](#) |
| sysu003  | Transverse   | Premium | 4-14 mm     | 3.5 m  | 10-30 mm | [Download](#) |
| sysu004  | Transverse   | Premium | 19-31 mm    | 9 m    | 6-20 mm  | [Download](#) |
| sysu005  | Transverse   | Premium | 5-7 mm      | 11.14 m | 50-100 mm & >100 mm | [Download](#) |
| sysu006  | Transverse   | Premium | 15-23 mm    | 12.09 m | 15-35 mm | [Download](#) |
| sysu007  | Transverse   | Premium | Avg. 30 mm  | 11.61 m | 20-40 mm | [Download](#) |
| sysu008  | Transverse   | Premium | 23-37 mm    | 11.78 m | >10 mm   | [Download](#) |
| sysu009  | Transverse   | Premium | 17 mm       | 11.86 m | 10-40 mm | [Download](#) |
| sysu010  | Alligator    | Premium | Max 100 mm  | 1.77 m | <17 mm   | [Download](#) |
| sysu011  | Longitudinal | Premium | 1.5-20 mm   | 5 m    | 3-14 mm  | [Download](#) |
| sysu012  | Longitudinal | Premium | >1 mm       | 4.87 m | 10 mm    | [Download](#) |
| sysu013  | Transverse   | Premium | 3-14 mm     | 12.11 m| Max 20 mm| [Download](#) |
| sysu014  | Longitudinal | Premium | 1-18 mm     | /      | Max 9.21 mm | [Download](#) |
| sysu015  | Block+Alligator | Premium | 3-42 mm | / | Max 27.28 mm | [Download](#) |
| sysu016  | Transverse   | Premium | 2.16-21.36 mm | / | 4.02-15.50 mm | [Download](#) |
| sysu017  | Transverse   | Premium | 1.58-30.87 mm | / | 2.40-10.90 mm | [Download](#) |
| sysu018  | Longitudinal | Premium | 3.61-21.23 mm | / | 6.8-14.55 mm | [Download](#) |
| sysu019  | Transverse   | Premium | 3.9-33.69 mm | / | 7.02-14.33 mm | [Download](#) |
| sysu020  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu021  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu022  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu023  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu024  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu025  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu026  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu027  | /            | Medium  | /           | /      | /         | [Download](#) |
| sysu028  | /            | Medium  | /           | /      | /         | [Download](#) |


## Usage Instructions
- **Viewing**: You can use CloudCompare, MeshLab, or Open3D to visualize and analyze the point cloud data.
- **Processing**: Python users can load the `.ply` files with Open3D:
  ```python
  import open3d as o3d
  pcd = o3d.io.read_point_cloud("crack_001.ply")
  o3d.visualization.draw_geometries([pcd])
  ```

## Citation
If you use this dataset in your research, please cite appropriately:
> Apple LiDAR Pavement Cracks Dataset, Sun Yat-sen University, Zhuhai Campus

## License
This dataset is provided for research purposes only. Please contact the dataset owner for any commercial use inquiries.
