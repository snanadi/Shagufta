![image](https://github.com/snanadi/Shagufta/assets/159690874/4b9ca4c5-284a-4f25-a386-d674969dc5fb)# ml project
Cancer Detection with Pydicom and K-means is a Python project aimed at utilizing medical imaging data in DICOM format to detect potential cancerous regions within medical scans.

Software requirements
1. Jupyter notebook.
2. pylidc is a python library intended to improve workflow associated with the LIDC dataset.
3. tensorflow 2

Setup Environment
From the obtained data set 80% was used as training set and 20% was kept as test set. This test 
set is completely kept out of the training process. Data analysis showed that there is much 
variance in the size and location of the nodules. Therefore, a model needs enough training 
examples to generalize well. On the other hand, there need to be enough test data to evaluate 
the models after training. Therefore, the 80:20 ratio is a reasonable choice. 
• Train (1): used in the training process. Contains training- and validation part.
• Test: used to test classifier. This subset is completely kept out of the training process.
• Validation: used to validate the classifier during the training process. Furthermore, used for 
stop- or improvement criteria

The dataset used is extracted from the LIDC/IDRI dataset. LIDC/IDRI is the largest publicly available reference database of chest CT scans. It consists of 1,018 thoracic CT scans collected from seven academic institutions with a wide range of scanner models and acquisition parameters [16]. CT images from each scan is associated with an XML file recording nodule reports and diagnosis reports of image annotation process from four experienced thoracic radiologists.
Each LIDC/IDRI annotation was created by a two-phase reading process. In the first blinded reading phase, suspicious lesions were independently annotated by four experienced thoracic radiologists as nodule >3 mm, nodule >3 mm, or non-nodule (any other pulmonary abnormality). In the second nonblind reading phase, the blinded results of all other radiologists were revealed to each radiologist, who then decided to accept or reject each annotation. No consensus was forced. The LIDC/IDRI annotations for nodules ≥3 mm include position, diameter of nodule in each CT slice, and subjective ratings on a five-point or six-point scale of the pathologic features: calcification, internal structure, subtlety, lobulation, margins, sphericity, malignancy, texture, and spiculation 

