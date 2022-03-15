# Multiclass Alzheimer Disease Prediction

## 1. Abstract
Alzheimer’s Disease is the most prevalent form of dementia with more than 30 million cases worldwide. AD is believed to be caused by the abnormal deposits of amyloid and tau proteins that form plaques and tangles in the brain. Diagnosis of early-onset AD is time-consuming, costly, and inaccurate because of the diverse nature of human intelligence and the inconsistencies in the observed symptoms. Nonetheless, significant advancements in neuroimaging technology combined with deep learning methodologies capable of identifying intricate features from complex data make it possible to design models capable of yielding high accuracies. The paper proposes an end-to-end deep learning model to identify and classify 2D MRI images of the brain into four categories depending on the presence and progression of the disease. The 2D MRI data is subjected to segmentation, noise removal, and feature extraction using Gabor filters. The proposed model has a neural network architecture consisting of Alexnet CNN combined with ReLU, softmax, and max-pooling layers. The model was trained using the Adam optimization algorithm and categorical sparse cross-entropy loss function. Findings from the research suggest that the proposed model is capable of delivering high accuracies with less amount of data and low computational power. The research also stands out as one among the few models capable of identifying the different stages of AD rather than a binary classification model.


## 2. Introduction
The concept of dementia as a disease associated with the old and exhibiting symptoms of progressive deterioration of cognitive skills has existed for centuries, however, it was only in 1907 that the first case of presenile dementia was reported. Aloysius Alzheimer carefully observed and recorded a series of strange behavioral symptoms exhibited by a 51-year-old patient at the Frankfurt Asylum. The type of dementia later came to be known as Alzheimer’s disease. Dementia is a syndrome that affects memory adversely whereas Alzheimer's disease is a chronic brain disorder that progressively leads to memory and cognitive decline.
Today, Alzheimer’s disease is known to be the most prevalent type of dementia and contributes to more than 60% of all reported cases, and is often characterized as an inevitable consequence of aging (Fig 1). Alzheimer’s disease is delineated as a degenerative brain disorder as the symptoms tend to aggravate with time. An early stage symptom associated with the disease is short-term memory. As the disease progresses, symptoms like language disturbance, disorientation, mood-swings, self-neglect and behavioral issues are observed extensively. Gradually, the Alzheimer's patient will struggle to perform day-to-day activities. Further on, losing his/her brain’s ability to perform life sustaining bodily functions, eventually leading to death.

## 2.1 Categories of Alzheimer’s Disease
There are three major stages of Alzheimer’s disease: 
Very Mild Demented: The onset of Alzheimer’s Disease from a neuropathological perspective begins long before any symptoms are observed. The very mild demented stage refers to the stage of mild cognitive impairment. Protein deposits of abnormal capacities are observed in the brain. Consequently, Plaques and tangles are starting to affect the areas of the brain associated with cognition.
Mildly Demented: This stage of Alzheimer’s disease is widely associated with the observed shrinkage in the size of brain at a degree greater than what is observed during healthy aging of a person. The plaques and tangles are noticed to spread to the other  cortical areas in a predictable pattern. Frequent memory lapses are observed because of the hippocampus being affected. 
Moderately demented: A substantial shrinkage of the size of the brain is observed because of the widespread damage of neurons. Plaques and tangles spreading to the major areas of the cortex causes significant changes in the personality and behavior exhibited by the patient.
Alzheimer’s disease further proceeds into the severely demented state as the brain tissues are fully damaged and the person loses the ability to function independently. Ultimately, proving fatal.

Despite the fact that Alzheimer’s disease is an irreversible, degenerative brain disorder, early stage diagnosis can go a long way in gradually slowing down and preventing the progression of the disease. However, an early stage diagnosis is all the more difficult as it requires several neurological and biological examinations and a study of the detailed history of the patient. Lately, detailed brain images generated using Magnetic Resonance Imaging (MRI), a non-invasive imaging technology has been identified as a nascent method for identifying Alzheimer’s disease. The observed shrinkage in the hippocampus and cerebral cortex and the enlargement of the vertices further enhances the potential of neuroimaging in identifying Alzheimer’s disease.

The possibility of errors and the time-consuming nature of manual examination of MRI images calls for an automated method for the segmentation and classification of brain images. Traditional machine learning models and shallow neural networks have been extensively tried and tested and have proved successful for the task. However, deep learning architectures capable of extracting intricate features from complex data are capable of tremendously improving the performance. This is evident from deep learning having shown superior performance in many real-world applications of computer vision in healthcare.

The research attempts to benefit the doctors, patients and the mental healthcare workers to identify the patterns of Alzheimer’s disease and to investigate if image processing using CNN can diagnose and interpret the stage of progression of neurobiological diseases like Alzheimer's.


## 2.2 EDA on Longitudinal MRI Data in Nondemented and Demented Older Adults
For performing the EDA the dataset used consisted of a selection of 150 subjects between 60 and 96 years of age. During a total of 373 imaging sessions, two or more samples were scanned for each subject and divided by at least a year. 3 or 4 T1 weighted MRI scans are used for each subject, obtained in single scans. The themes are all correct and involve men and women alike. During the entire study, 72 of the subjects were identified as undemanded. At their initial visits, 64 patients, including 51 people suffering from slight to severely high Alzheimer's disease, were characterised as demented and remained so for subsequent scans.

After applying data cleaning and processing it was observed that
There are about 39% demented cases in the dataset i.e., majority of the data is of Non Demented scenarios while 10% of the dataset is of Converted.

Furthermore, using the CDR scores it can be derived that the majority of the cases are Normal while many cases are of Mild and Moderate dementia.

 
Note: The Non-Demented classification is for the MRI images of cases without Alzheimer’s disease. 

## Conclusion
Our findings show that transfer learning on a small scale training dataset for AD-prediction based on structural brain fMRI scans is a possible appropriate method for the training of CNN classifier. Pre-Trained convolutional layers, such as convolutional AlexNet layers pretrained on ImageNet, could extract generic imaging features and could provide good feedback for the subsequent AD classification neural network with high accuracy of 86.54%. AlexNet has thus resulted in a lightweight efficient model that could further potentially revolutionise the field of medical sciences with its implementation in various clinics, hospitals, etc.
 
Future Research directions
 
Here are the various improvisation which can be suggested for the architecture-
Increasing Dataset - Amount of Training Data needs to be increased as accuracy is proportional to the number of training images in the dataset.
Addition of More Layers - More feature extraction layers needs to be added in the architecture along with the pooling and activation layers - ReLu, Softmax for better optimization and training as additional layers will allow the network to learn more complex classification and thereby improve class performance.
Increasing / Decreasing Image Size - While pre-processing the images for training and evaluation, image sizes need to be regulated as a smaller image size will prevent the extraction of distinctive features while larger images may not have enough data to may not be complex enough for the model to process them.
Increasing the Training Time - The model was initially trained on 100 epochs thereby additional epoch intervals  of +25,+50, +100, etc can boost classifier's performance until at one point of time on increasing  training time accuracy cannot be improved. Thus optimal learning rate parameters needs to be experimented with to improve the performance of the model.
 
