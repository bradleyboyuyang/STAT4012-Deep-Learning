## Face Detection
Realize the classic computer vision task: face detection and recognition using Bollywood celebrity faces.

### Source Data
We pick a part of (more than 1000 observations) the [Bollywood celebrity faces](https://www.kaggle.com/datasets/havingfun/100-bollywood-celebrity-faces)  from Kaggle for face recognition purposes. The raw data contains images of different sizes for 13 different Bollywood celebrities. 

### Models
Faces will be explored using Haar-like Classifiers in OpenCV. Features will be extracted using MTCNN. Classification tasks are finished using self-built CNNs and pre-trained models in Keras such as AlexNet and ResNet. Eventually FaceNet will be used to obtain embeddings and celebrities are classified using a simple SVM or MLP. We use the renowned pre-trained FaceNet keras model (in h5 format) which is available online.

### Scripts
- `MTCNN.ipynb`: Using MTCNN to detect the location and information of the faces.
- `CNN.ipynb`: Basic exploratory data analysis and self-built CNN models.
- `EDA-FaceNet.ipynb`: Part of exploratory image visualization and SVM classification using FaceNet embeddings.
- `keras_models.ipynb`: Face detection using well-known pre-trained image recognition models in Keras.
- `FaceNet.ipynb`: FaceNet employment and performance measure.

#### Haar-like Classifiers

<img src="./final_report/figures/har2.png" width="650">

#### MTCNN Structure

<img src="./final_report/figures/mtcnn1.png" width="750">

#### FaceNet Structure

<img src="./final_report/figures/facenetX.png" width="750">

### Results
#### Train-test Proportions

<img src="./final_report/figures/train_test.png" width="750">

#### Samples of the Correctly Labeled Images

<img src="./final_report/figures/correct.png" width="650">

#### Samples of the Incorrectly Labeled Images

<img src="./final_report/figures/mislabeled.png" width="650">

#### Accuracy/Loss of a Self-built CNN

<img src="./final_report/figures/cnn2.png" width="750">


#### Accuracy of a Keras Built-in Model

<img src="./final_report/figures/res1.jpg" width="750">


#### Loss of a Keras Built-in Model

<img src="./final_report/figures/res2.jpg" width="750">

#### Confusion Matrix of FaceNet + SVM on Test Dataset

<img src="./final_report/figures/svm_confusion_test.png" width="700">
