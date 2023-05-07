# Quality-Evaluation-of-Skull-Stripped-Brain-MRI-Images
Skull stripped brain MRI images are usually shared in open
access data repositories for collaboration and knowledge dis-
semination in order to advance neuro imaging research. Skull
stripping is a process of removing the image voxels that repre-
sent the skull structure and facial features from raw 3D MRI
images to ensure HIPAA compliance. Sometimes, the facial
features are still in the processed images, and the other times,
the voxels representing actual brain tissues are removed. To
ensure the quality of the skull stripping process, researchers
often spend a lot of time and effort to inspect the quality of
the segmentation results. This paper suggests a deep neural
network algorithm which makes the inspection of the skull
stripped MRI images easy and reduces the manual interven-
tion. The deep neural network algorithm which is explored
in this paper is 3D Convolutional Neural Networks(CNN).
CNNs makes it easy to process the images and evaluates the
quality of skull stripped images with a good accuracy.

---
### Data set
The `BET_BSE` dataset can be downloaded from [this](https://dyslexia.computing.clemson.edu/BET_BSE/) link. The dataset contains 2060 brain MRI image files and a lables.csv file. The brain MRI images are of [NIFTI](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwim1OSJh-T-AhV5nGoFHQFDAOYQjBB6BAgMEAE&url=https%3A%2F%2Fnifti.nimh.nih.gov%2Fnifti-1%2F&usg=AOvVaw0VSywKKASUHDZWjCMAhcJ2) format. The lables.csv contains the lables for each image in the dataset. The labels for each image include `Recognizable Facial Features` and `Brain Feature Loss`.



---

### Contributors
* Shareef Shaik
* Tejaswine Kantu
