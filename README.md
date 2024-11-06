## Team
Francisco Lozano – Graduate student 

## Type of project
Implementation project 

## Description
The objective of this project is to develop and evaluate an automated driver drowsiness detection system using facial analysis. This project aims to enhance road safety by identifying drowsy driving behavior and alerting the driver. Using image processing and machine learning we can accurately detect signs of drowsiness based on facial features, such as eye closure duration. By continuously monitoring these indicators through a camera feed, the system should be able to detect early signs of drowsiness and issue alerts before driving impairment occurs. As proof of concept, the system will first scan an image of a person’s face and establish a baseline. Then, through a graphical user interface (GUI), an additional image of the same person will be inputted to simulate drowsiness detection. The system will analyze this image and indicate whether signs of drowsiness are detected. 

## Directory setup
- data: folder that contains the raw & preprocessed data for the project  
- output: contains outputs such as data/graphs needed for the project - these outputs are generated by the jupyter notebooks  
- src: contains reusable code imported by the notebooks 
- app: contains the source code for the gradio app in HuggingFace
- images: containes images used by notebooks for reporting (This DOES NOT include images used for TRAIN/TEST)
- models: contains models used or generated by the notebooks.

## Proposed Methodology and Techniques: 

1. Data Collection: Gather datasets of drivers under different levels of drowsiness. 

2. Preprocessing: Use image processing techniques to normalize images, detect facial landmarks, and isolate critical features like eyes. This is where the image processing techniques learned in class will be applied. 

3. Model Development: Train and evaluate different machine learning models (ex; Support Vector Machine) to classify drowsiness levels based on eye closure. 

4. Implementation and Testing: Develop a Python-based GUI for classification, integrating the drowsiness detection model. Test the system on a set of labeled images to ensure accurate detection. 

## Dataset

https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd

## App Deployment
I deployed my final model in HuggingFace via a gradio app. [Check it out!]() TODO

## References: 

- A Review of Recent Developments in Driver Drowsiness Detection Systems, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8914892/ 
- Driver drowsiness monitoring system using visual behaviour and machine learning, https://ieeexplore.ieee.org/document/8405495 
- Drivers Drowsiness Detection using Image Processing and I-Ear Techniques, https://ieeexplore.ieee.org/document/10142501 
- X. Guo, "LIME: A Method for Low-light Image Enhancement," Proceedings of the 24th ACM International Conference on Multimedia, Amsterdam, The Netherlands, 2016, pp. 87-91, doi: 10.1145/2964284.2967188. https://doi.org/10.1145/2964284.2967188
- Fei Ni, Zhuang Fu, QiXin Cao, YanZheng Zhao. “Image processing method for eyes location based on segmentation texture”. Sensors and Actuators A: Physical, Volume 143, Issue 2, 2008, Pages 439-451. ISSN 0924-4247. https://doi.org/10.1016/j.sna.2007.11.033.
- Albadawi Y, Takruri M, Awad M. “A Review of Recent Developments in Driver Drowsiness Detection Systems”. Sensors (Basel). 2022 Mar 7;22(5):2069. doi: 10.3390/s22052069. PMID: 35271215; PMCID: PMC8914892.
- M. A. Faidhi Daud, A. P. Ismail, N. M. Tahir, K. Daud, N. M. Kasim and F. A. Mohamad, "Real Time Drowsy Driver Detection Using Image Processing on Python," 2022 IEEE 12th International Conference on Control System, Computing and Engineering (ICCSCE), Penang, Malaysia, 2022, pp. 131-136, doi: 10.1109/ICCSCE54767.2022.9935627.
- A. Kumar and R. Patra, "Driver drowsiness monitoring system using visual behaviour and machine learning," 2018 IEEE Symposium on Computer Applications & Industrial Electronics (ISCAIE), Penang, Malaysia, 2018, pp. 339-344, doi: 10.1109/ISCAIE.2018.8405495.
- Nasri, I., Karrouchi, M., Snoussi, H., Kassmi, K., Messaoudi, A. (2022). Detection and Prediction of Driver Drowsiness for the Prevention of Road Accidents Using Deep Neural Networks Techniques. In: Bennani, S., Lakhrissi, Y., Khaissidi, G., Mansouri, A., Khamlichi, Y. (eds) WITS 2020. Lecture Notes in Electrical Engineering, vol 745. Springer, Singapore. https://doi.org/10.1007/978-981-33-6893-4_6
- Kazemi, V., & Sullivan, J. (2014). One millisecond face alignment with an ensemble of regression trees. 2014 IEEE Conference on Computer Vision and Pattern Recognition, 1867-1874. https://www.semanticscholar.org/paper/One-millisecond-face-alignment-with-an-ensemble-of-Kazemi-Sullivan/d78b6a5b0dcaa81b1faea5fb0000045a62513567?p2df 

## TODO List

Make a seperate notebook for each item 1-5.

1. [X] Preprocess the images to show the eye features more. THIS IS THE MEAT OF THE PROJECT.
1. [ ] Use Python, OpenCV, and dlib code to (1) perform facial landmark detection and (2) detect blinks in preprocesed images. THIS IS THE MEAT OF THE PROJECT.
1. [ ] Improve the detect blinks using a SVM.
1. [ ] Build a drowsiness detector, by monitoring the eye aspect ratio (given by blink detector) to see if the value falls but does not increase again, thus implying that the person has closed their eyes.
1. [ ] Turn everything into a video stream analyzer.
1. [ ] Build a gradio app implementing the system for a better UI/UX experience.
1. [ ] Make the presentation.
1. [ ] Write the Final report.

