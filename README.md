# DENTEX CHALLENGE 2023 
Dental Enumeration and Diagnosis on Panoramic X-rays Challenge


<details><summary>Table of Contents</summary><p>
  
* [What is DENTEX?](#what-is-dentex)
* [Desired Output of the Challenge](#desired-output-of-the-challenge)
* [Data](#data)
* [Citing Us](#citing-us)
* [License](#license)
* [Contact](#contact)
  
</p></details><p></p>


## What is DENTEX?
We present the Dental Enumeration and Diagnosis on Panoramic X-rays Challenge (DENTEX), organized in conjunction with the International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI) in 2023. The primary objective of this challenge is to develop algorithms that can accurately detect abnormal teeth with dental enumeration and associated diagnosis. This not only aids in accurate treatment planning but also helps practitioners carry out procedures with a low margin of error.

The challenge provides three types of hierarchically annotated data and additional unlabeled X-rays for optional pre-training. The annotation of the data is structured using the Fédération Dentaire Internationale (FDI) system. The first set of data is partially labeled because it only includes quadrant information. The second set of data is also partially labeled but contains additional enumeration information along with the quadrant. The third data is fully labeled because it includes all quadrant-enumeration-diagnosis information for each abnormal tooth, and all participant algorithms will be benchmarked on the third data. 

DENTEX aims to provide insights into the effectiveness of AI in dental radiology analysis and its potential to improve dental practice by comparing frameworks that simultaneously point out abnormal teeth with dental enumeration and associated diagnosis on panoramic dental X-rays.

*Please visit our website to join [DENTEX (Dental Enumeration and Diagnosis on Panoramic X- rays Challenge)](https://dentex.grand-challenge.org/) which is held at MICCAI2023.*

## Desired Output of the Challenge
![Fig. 1. A desired output from a final algorithm, illustrating well-defined bounding boxes for each abnormal tooth. The corresponding quadrant (Q), enumeration (N), and diagnosis (D) labels are also displayed.](figures/output.png)
*Fig. 1. A desired output from a final algorithm, illustrating well-defined bounding boxes for each abnormal tooth. The corresponding quadrant (Q), enumeration (N), and diagnosis (D) labels are also displayed.*


## Data
![Fig. 2. The hierarchical organization of the annotated data. The data is structured into three levels: (a) quadrant-only for quadrant detection, (b) quadrant-enumeration for tooth detection, and (c) quadrant-enumeration-diagnosis for abnormal tooth detection.](figures/data.png)
*Fig. 2. The hierarchical organization of the annotated data. The data is structured into three levels: (a) quadrant-only for quadrant detection, (b) quadrant-enumeration for tooth detection, and (c) quadrant-enumeration-diagnosis for abnormal tooth detection.*

The DENTEX dataset comprises panoramic dental X-rays obtained from three different institutions using standard clinical conditions but varying equipment and imaging protocols, resulting in diverse image quality reflecting heterogeneous clinical practice. The dataset includes X-rays from patients aged 12 and above, randomly selected from the hospital's database to ensure patient privacy and confidentiality.

To enable effective use of the FDI system, the dataset is hierarchically organized into three types of data;

        (a) 693 X-rays labeled for quadrant detection and quadrant classes only,

        (b) 634 X-rays labeled for tooth detection with quadrant and tooth enumeration classes,

        (c) 1005 X-rays fully labeled for abnormal tooth detection with quadrant, tooth enumeration, and diagnosis classes.

The diagnosis class includes four specific categories: caries, deep caries, periapical lesions, and impacted teeth. An additional 1571 unlabeled X-rays are provided for pre-training. 

* The dataset is used for [DENTEX (Dental Enumeration and Diagnosis on Panoramic X-rays Challenge)](https://dentex.grand-challenge.org/). 

**Note**: The datasets are fully identical to the data used for our baseline method named as HierarchicalDet. Therefore, please visit [HierarchicalDet (iffusion-Based Hierarchical Multi-Label Object Detection to Analyze Panoramic Dental X-rays)](https://github.com/ibrahimethemhamamci/HierarchicalDet) repo for more info.

## Citing Us

If you use DENTEX, we would appreciate references to the following papers. 

1. **Ibrahim Ethem Hamamci, Sezgin Er, Enis Simsar, Anjany Sekuboyina, Mustafa Gundogar, Bernd Stadlinger, Albert Mehl, Bjoern Menze., Diffusion-Based Hierarchical Multi-Label Object Detection to Analyze Panoramic Dental X-rays, 2023.**<br  />Pre-print: https://arxiv.org/abs/2303.06500


## License
The data is provided under the [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/), making it fully open-sourced.

The rest of this repository is under the [MIT License](https://choosealicense.com/licenses/mit/).


## Contact
For queries and issues not fit for a github issue, please email [Ibrahim Ethem Hamamci](mailto:ibrahim.hamamci@uzh.ch).
