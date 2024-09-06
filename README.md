<h1>102 Flowers Recognition</h1>
This project involves a task of image classification of flowers using the 102 Category Flower Dataset(link). This dataset is characterized by having an unusual division of train, validation, and test sets, with small train and validation sets (1020 images) and a very large test set (6149 images). The goal of this work is to create a high-performance model while maintaining the unusual split of the dataset and to make it as lightweight as possible, so as to enable deployment on devices with limited resources. Three models were implemented using the principles of transfer learning, namely by performing feature extraction and fine tuning using three different models pretrained on ImageNet (VGG16, InceptionV3, ResNet50). Once the most performant model was identified, a model explanation was conducted implementing grad-CAM and LIME, to understand and demonstrate the functioning of the model, and quantization was performed in float-32, float-16, and int-8. The work thus demonstrates that, despite the dataset having unusual and suboptimal train, validation, and test set splits, it is still possible to obtain a high-performance model, with an accuracy of about 86%, and compressed, with a significant reduction in terms of memory from 80MB to 11MB without compromising on performance.

<h2>How to use</h2>
The notebooks for this work have been written and executed on the Kaggle platform. Below is how to run the notebooks.

<h3>Kaggle</h3>
1. Download the 'aml_flowers-dataset' folder from the drive.
2. Log in to your Kaggle account.
3. Go to the dropdown menu on the left and navigate to the 'Dataset' section. In this section, click 'New Dataset' and drag the dataset folder into the Drag & Drop cell that opens. (Note: the folder must be compressed before importing it as otherwise it is too large and cannot be imported). Choose a title, set the visibility, and finally click 'Create' and 'Go to the dataset'.
4. On the page that opens, click 'New notebook'. This will open the notebook with the dataset already loaded. Otherwise, create a new notebook by going to the left menu and selecting 'Code', 'New notebook'. Once the notebook is open, go to the right menu in the 'Data' section. Click 'Add data', 'Your dataset', and import the newly created dataset.
5. Once the dataset is imported, import the notebook by doing file->import notebook and select the notebook to open.
6. Start the session by selecting in 'notebook options -> accelerator' in the right menu, GPU T4 x2. If this is your first time logging into Kaggle, you need to enter your phone number. To do this, go to the right menu, 'notebook options'. Under 'Add Tags' there is a link 'Get phone verified'. After the procedure, you will be able to use the accelerator.
7. Once the session starts, check that the paths in cell number two are correct to work on the dataset.
8. Click 'Run all'


