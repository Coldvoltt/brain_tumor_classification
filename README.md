## brain_tumor_classification
The brain tumor MRI dataset, which is accessible at [this URL] (https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset), 
provided the MRI scan images required for this work. The dataset consists of a collection of 7023 MRI scans of the human brain that represent 
a wide range of situations. **Glioma**, **meningioma**, **no_tumor**, and **pituitary** are the four separate classes into which these photos 
have been divided. Asides from the no_tumor class which are classes without tumors, each class reflects a particular kind of brain disorder, 
enabling thorough analysis and evaluation. The dataset's wide range and quantity make it a priceless tool for this research.  

We employ the Convolutional Neural Network (CNN) with multiple layers and some activation functions. 

In the modeling phase, we partition our data into train and test sets in the ratio of 80:20. This CNN model we built has several layers, each of which has a unique set of parameters. 
**More detains in the notebook**.

## Summary
The model performed well overall, as seen by its training accuracy of 0.99 and loss of 0.01 and validation accuracy of 0.89, and a validation loss of 0.5. However, we found that the model's performance, notably in classifying glioma, was below average.
We created a confusion matrix to examine the model's performance in more detail. We noticed from the confusion matrix that the model had trouble correctly classifying glioma cases. This shows that there might be a problem with class imbalance or insufficient glioma sample representation in the training data. Due to its complex features or resemblances to other brain structures, glioma may be a more difficult class to detect. To solve this issue, we may consider collecting more glioma samples.  

In summary, the CNN model performs admirably overall, with high accuracy and minimal loss. However, more work needs to be done to accurately classify gliomas. To achieve an overall accurate classification across all classes in the brain MRI scans, further optimization and refinement may be required, as well as a sufficient representation of glioma samples.
