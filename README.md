# Chest_X-Ray_Medical_Diagnosis_with_Deep_Learning
Project Description
The project uses a pretrained DenseNet-121 model able to diagnose 14 labels such as Cardiomegaly, Mass, Pneumothorax or Edema. In other words, this single model can provide binary classification predictions for each of the 14 labeled pathologies.

Weight normalization is performed to offset the low prevalence of the abnormalities among the dataset of X-Rays (class imbalance).

Finally the GradCAM technique is used to highlight and visualize where the model is looking, which area of interest is used to make the prediction. This is a tool which can be helpful for discovery of markers, error analysis, training and even in deployment.

Dataset
The project uses chest x-ray images taken from the public ChestX-ray8 dataset. This dataset contains 108,948 frontal-view X-ray images of 32,717 unique patients. Each image in the data set contains multiple text-mined labels identifying 14 different pathological conditions. These in turn can be used by physicians to diagnose 8 different diseases. For the project we have been working with a ~1000 image subset of the images.

875 images to be used for training.
109 images to be used for validation.
420 images to be used for testing.
The dataset includes a CSV file that provides the ground truth labels for each X-ray.
Model settings
In this project, the model uses 320 x 320 X-Rays images and outputs predictions for each of the 14 pathologies as illustrated below on a sample image.
