# ml project
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
