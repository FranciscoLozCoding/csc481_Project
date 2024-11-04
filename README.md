## Team
Francisco Lozano – Graduate student 

## Type of project
Implementation project 

## Description
The objective of this project is to develop and evaluate an automated driver drowsiness detection system using facial analysis. This project aims to enhance road safety by identifying drowsy driving behavior and alerting the driver. Using image processing and machine learning we can accurately detect signs of drowsiness based on facial features, such as eye closure duration. By continuously monitoring these indicators through a camera feed, the system should be able to detect early signs of drowsiness and issue alerts before driving impairment occurs. As proof of concept, the system will first scan an image of a person’s face and establish a baseline. Then, through a graphical user interface (GUI), an additional image of the same person will be inputted to simulate drowsiness detection. The system will analyze this image and indicate whether signs of drowsiness are detected. 

## Proposed Methodology and Techniques: 

1. Data Collection: Gather datasets of drivers under different levels of drowsiness. 

2. Preprocessing: Use image processing techniques to normalize images, detect facial landmarks, and isolate critical features like eyes. This is where the image processing techniques learned in class will be applied. 

3. Model Development: Train and evaluate different machine learning models (ex; Support Vector Machine) to classify drowsiness levels based on eye closure. 

4. Implementation and Testing: Develop a Python-based GUI for classification, integrating the drowsiness detection model. Test the system on a set of labeled images to ensure accurate detection. 

## References: 

- A Review of Recent Developments in Driver Drowsiness Detection Systems, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8914892/ 
- Driver drowsiness monitoring system using visual behaviour and machine learning, https://ieeexplore.ieee.org/document/8405495 
- Drivers Drowsiness Detection using Image Processing and I-Ear Techniques, https://ieeexplore.ieee.org/document/10142501 
- X. Guo, "LIME: A Method for Low-light Image Enhancement," Proceedings of the 24th ACM International Conference on Multimedia, Amsterdam, The Netherlands, 2016, pp. 87-91, doi: 10.1145/2964284.2967188. https://doi.org/10.1145/2964284.2967188
- Fei Ni, Zhuang Fu, QiXin Cao, YanZheng Zhao. “Image processing method for eyes location based on segmentation texture”. Sensors and Actuators A: Physical, Volume 143, Issue 2, 2008, Pages 439-451. ISSN 0924-4247. https://doi.org/10.1016/j.sna.2007.11.033.
- Albadawi Y, Takruri M, Awad M. “A Review of Recent Developments in Driver Drowsiness Detection Systems”. Sensors (Basel). 2022 Mar 7;22(5):2069. doi: 10.3390/s22052069. PMID: 35271215; PMCID: PMC8914892.
- M. A. Faidhi Daud, A. P. Ismail, N. M. Tahir, K. Daud, N. M. Kasim and F. A. Mohamad, "Real Time Drowsy Driver Detection Using Image Processing on Python," 2022 IEEE 12th International Conference on Control System, Computing and Engineering (ICCSCE), Penang, Malaysia, 2022, pp. 131-136, doi: 10.1109/ICCSCE54767.2022.9935627.
- A. Kumar and R. Patra, "Driver drowsiness monitoring system using visual behaviour and machine learning," 2018 IEEE Symposium on Computer Applications & Industrial Electronics (ISCAIE), Penang, Malaysia, 2018, pp. 339-344, doi: 10.1109/ISCAIE.2018.8405495.

