# Quality-Evaluation-of-Skull-Stripped-Brain-MRI-Images
Skull stripped brain MRI images are usually shared in open
access data repositories for collaboration and knowledge dissemination in order to advance neuro imaging research. Skull
stripping is a process of removing the image voxels that represent the skull structure and facial features from raw 3D MRI
images to ensure HIPAA compliance. Sometimes, the facial
features are still in the processed images, and the other times,
the voxels representing actual brain tissues are removed. To
ensure the quality of the skull stripping process, researchers
often spend a lot of time and effort to inspect the quality of
the segmentation results. This paper suggests a deep neural
network algorithm which makes the inspection of the skull
stripped MRI images easy and reduces the manual intervention. The deep neural network algorithm which is explored
in this paper is 3D Convolutional Neural Networks(CNN).
CNNs makes it easy to process the images and evaluates the
quality of skull stripped images with a good accuracy.

---
### Dataset
The `BET_BSE` dataset can be downloaded from [this](https://dyslexia.computing.clemson.edu/BET_BSE/) link. The dataset contains 2060 brain MRI image files and a lables.csv file. The brain MRI images are of [NIFTI](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwim1OSJh-T-AhV5nGoFHQFDAOYQjBB6BAgMEAE&url=https%3A%2F%2Fnifti.nimh.nih.gov%2Fnifti-1%2F&usg=AOvVaw0VSywKKASUHDZWjCMAhcJ2) format. The lables.csv contains the lables for each image in the dataset. The labels for each image include `Recognizable Facial Features` and `Brain Feature Loss`.

---
### How to run the code?
* **Step 1:** Download the dataset from the link provided in the Dataset section. The dataset folder will be named as `BSE_BET_DATA`. The folder `BSE_BET_DATA` contains a subfolder called `files` and a labels.csv.
* **Step 2:** Download the `Quality_Evalution_Model.ipynb` and place inside the folder `BSE_BET_DATA`.
* **Step 3:** Execute each cell of the `Quality_Evalution_Model.ipynb` file. The 3D convolutional model will be build and will be trained for 35 epcohs. After the model is trained, it will be saved inside a folder named `Model`. (`Note:` Make sure to create a folder called `Model` to save the trained model). In later steps the saved model is loaded and evaluated using test dataset. 

At the end, the model accuracies(ie.e., train, validation and test accuracies) are also saved and loaded to plot the `accuracy vs epoch` graph. 

 
---

### Contributors
* [Shareef Shaik](https://github.com/skshareef)
* Tejaswine Kantu
