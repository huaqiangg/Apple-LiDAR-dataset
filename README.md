# Apple LiDAR Pavement Cracks Dataset

## Overview
This dataset consists of crack point clouds collected at the Zhuhai campus of Sun Yat-sen University using the LiDAR on Apple devices. The dataset is intended for research on the potential application of Apple LiDAR in pavement crack detection.

## Data Collection Details
- **Device**: iPad pro 2021 or iPhone 16 Pro or ipad pro 2022
- **Software**: SiteScape —— LIDar 3D scanner 
- **Point Cloud Density**: ultra
- **Point Cloud Size**: Small  
- **File Format**: .ply  
- **Each File Represents**: A single crack  

## Crack Measurement Attributes
- **Crack Type Annotation**: Crack types (**transverse, longitudinal, alligator, and block cracks**) were manually labeled based on visual inspection.  
- **Weather Conditions**: Data was collected during **light rain**, and the point cloud may include water accumulation in cracks.  
- **Measurement Consistency**: All measurements were conducted by the **same team** to ensure consistency.  

## 📍 Crack Collection Locations
The image below shows the collection locations of different point cloud samples:
![](点云分布.png)


## Dataset Download
The dataset is available for download at the following link.
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17838389.svg)](https://doi.org/10.5281/zenodo.17838389)
| Crack ID | Crack Type | Density  |
|----------|------------|----------|
| sysu001  | Longitudinal | ultra |
| sysu002  | Transverse   | ultra | 
| sysu003  | Transverse   | ultra | 
| sysu004  | Transverse   | ultra | 
| sysu005  | Transverse   | ultra | 
| sysu006  | Transverse   | ultra | 
| sysu007  | Transverse   | ultra | 
| sysu008  | Transverse   | ultra | 
| sysu009  | Transverse   | ultra | 
| sysu010  | Alligator    | ultra | 
| sysu011  | Longitudinal | ultra |
| sysu012  | Longitudinal | ultra | 
| sysu013  | Transverse   | ultra |
| sysu014  | Longitudinal | ultra | 
| sysu015  | Transverse   | ultra | 
| sysu016  | Transverse   | ultra | 
| sysu017  | Transverse   | ultra |
| sysu018  | Transverse   | ultra | 
| sysu019  | Transverse   | ultra | 
| sysu020  | Transverse   | ultra | 
| sysu021  | Transverse   | ultra | 
| sysu022  | Transverse   | ultra | 
| sysu023  | Transverse   | ultra | 
| sysu024  | Transverse   | ultra | 
| sysu025  | Transverse   | ultra |
| sysu026  | Transverse   | ultra | 
| sysu027  | Transverse   | ultra | 
| sysu028  | Transverse   | ultra | 
| sysu029  | Transverse   | ultra | 
| sysu030  | Transverse   | ultra | 


We also acquired four sets of comparative point clouds for the same crack using seven different acquisition methods: 
handheld (at heights of 30 cm, 50 cm, and 70 cm);
gimbal-mounted (at heights of 30 cm, 50 cm, and 70 cm);
and Terrestrial Laser Scanning (TLS).
The dataset is available for download at the following link.
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17839334.svg)](https://doi.org/10.5281/zenodo.17839334)

| Crack ID | Crack Type | Density  |
|----------|------------|----------|
| control1  | Longitudinal | ultra |
| control2  | Transverse   | ultra | 
| control3  | Transverse   | ultra | 
| control4  | Transverse   | ultra | 



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
