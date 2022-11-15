# Introduction

Breast cancer is one of the major tumor-related causes of death in women. About 1 in 8 women will get breast cancer some time during their lifetime. The main methods of breast cancer diagnosis include ultrasound, mammography, and Magnetic Resonance Imaging (MRI). Digital Breast Tomosynthesis (DBT) is an advanced breast cancer screening technology approved by the FDA in 2011. DBT is often referred to as 3D Mammography since it produces quasi–three-dimensional (3D) images of the breast. In DBT, an X-ray machine is rotated to capture images of the breast tissue from different angles. These methods for diagnosis are crucial because early detection increases the survival rate by 8%. That is why mammograms are suggested for every woman over the age of 50 every 6 months. However, even experienced radiologists face problems in spotting micro-calcifications, lumps and masses. This leads to high false positives and high false negatives.

With the rapid progress of artificial intelligence (AI) techniques, along with digitalization in medicine science, physicians and patients believe adopting such technologies can be beneficial (Emiroglu et al., 2022). Deep learning techniques learn by creating an abstract representation of the data and therefore leads to higher accuracy results. The use of deep learning to analyze medical images and improve the accuracy of disease diagnosis is a rapidly growing area of interest. Until now deep learning has efficiently generated models that predict and classify different diseases. This process includes image and data analysis, and can be applied to different diseases such as breast cancer, liver disease, colon cancer, brain tumor, skin cancer, lung cancer, pneumonia and COVID-19.

Up until now, there has been some introduction of deep learning techniques into breast cancer diagnosis. Several studies until now have trained breast cancer data sets in order to analyze data with great accuracy. They used methods such as ImageNet and ResNet, which gives us an understanding that this is an active field and more research has to be done in order to further use these techniques for diagnostic purposes.
For this study, we will combine the diagnostic tools for breast cancer and deep learning methods. This will help with the accuracy of the diagnoses that patients get. The data provided by Cancer Imaging Archive consists of tomosynthesis data. For this study we will be using ResNet50, VGG, and Inception in order to classify tomosynthesis data.

# Motivation

Even though there is a lot of research that incorporates machine learning methods and medical diagnoses, at the moment there are not a lot of studies that incorporate machine learning methods with analyzing tomosynthesis data. Also, the research that is being done is not actively used for diagnosis purposes. This is due to the low relative accuracy that is obtained from the models.

The analysis of tomosynthesis data is time-consuming and challenging and certain conclusions can be very subjective. This will lead to patients potentially getting the wrong diagnosis. That is why in order to save money and time and increase the accuracy of such a process, it should be very desirable to automate the process by using machine learning techniques.

Buda et al., (2021) used the same data we have used to develop a baseline deep learning model for breast cancer detection and performed a deep learning algorithm based on DenseNet, and achieved 65% sensitivity on the test set.
This study is a clear implication that the aim and goal of our project are feasible and doable.

# Pre-processing

Using helper function provided from Duke University for preprocessing, details can be obtained from [here](https://github.com/ChloeZhou1997/BreastCancerCNN/blob/main/Preprocessing.ipynb).

# Model training and evaluation

The data is collected from Data Imaging Archives. The archive is accumulated from 5,610 studies for 5,060 participants for a total of 22,302 images. These are breast tomosynthesis images that include normal, actionable, biopsy-proven benign and biopsy-proven cancer cases; and there are a total of 2 classes: normal and all the abnormal cases combined. We used 3 different models for the classification: ResNet50, VGG and Inception. Since there are only 900 cancer images, we duplicated the cancer cases to match the number of normal images in the whole dataset. 80% of the data is divided as a training set and 20% of the data is used as a test set.

The training details and evaluation results can be obtained from:
- [ResNet](https://github.com/ChloeZhou1997/BreastCancerCNN/blob/main/Breast_Cancer_Detection_Project_ResNet.ipynb)
- [Inception](https://github.com/ChloeZhou1997/BreastCancerCNN/blob/main/Breast_Cancer_Classfication_inception.ipynb)
- [VGG](https://github.com/ChloeZhou1997/BreastCancerCNN/blob/main/Breast_Cancer_Classfication_VGG_v1.ipynb)
