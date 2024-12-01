# CNN Skin Cancer Detection Project

## Dataset
The dataset used in this project is the **Skin Cancer MNIST: HAM10000** dataset, which contains thousands of labeled dermoscopic images of various skin lesion types, including melanoma and basal cell carcinoma.

You can download the dataset from the following link: [HAM10000 Dataset](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)

After downloading, place the dataset in the `data/` directory of this project.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/CNN_Skin_Cancer.git
    cd CNN_Skin_Cancer
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Download the dataset and place it in the `data/` directory.

## Usage

### 1. Preprocessing the Dataset
Before training, the images need to be preprocessed. This step involves:
- Resizing images to a fixed size (e.g., 224x224 pixels)
- Normalizing pixel values
- Augmenting the dataset to improve the model's generalization

Run the following command to preprocess the images:
```bash
python preprocess.py
```
###2. Training the Model
To evaluate the model on a test dataset, use:
```bash
python evaluate.py
```
This will generate evaluation metrics such as accuracy, precision, recall, F1-score, and confusion matrix.

###4. Make Predictions
Once the model is trained, you can use it to make predictions on new skin lesion images. Use the following command:
```bash
python predict.py --image path_to_image
```
This will output the predicted label (malignant or benign) and the associated probability.


