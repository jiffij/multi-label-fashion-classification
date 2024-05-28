Name: Lu Cheuk Fung Jeff 
ID: G2304245F
CodaLab user name: clu014

*Caution* 
1. If you are want to print the "prediction.txt", please remove or rename the any file have the same name in the repository.
2. Please place the FashionDataset file at the root directory. Otherwise, please change variables IMG_DIR and SPLIT_DIR.
3. If you don't have all package yet, run "pip install -r requirements.txt".

All necessary code is contained in the jupyter notebook named "main.ipynb". 
The result of the validation accuracy will appear under the box called Evaluating Validation Accuracy.


Below are the variables need to change when producing the result.

Each time just have to press Run All. All script will run automatically.

Default option will calculate the validation accuracy and print the prediction.txt.

TRAINING = False # True: training
EVALUATE = True # True: calculate the validation loss and accuracy
PRINTING = True # True: print the 'prediction.txt'
MODEL_NAME = "<Please specify>" # The checkpoint file name if you are training a model
LOAD_CHECKPOINT = 'Swin_large_68_cont_best.pth' # This will be the checkpoint path used if you are evaluation or printing
IMG_DIR = os.path.join("FashionDataset", "FashionDataset","img")# The directory of images of the dataset, default "FashionDataset/FashionDataset/img" 
SPLIT_DIR = os.path.join("FashionDataset", "FashionDataset","split")  # The directory of the labels of the dataset, default "FashionDataset/FashionDataset/split"


--Reference--
timm: https://timm.fast.ai
pandas: https://pandas.pydata.org
Pillow: https://pillow.readthedocs.io/en/stable/
pytorch: https://pytorch.org
torchvision: https://pytorch.org/vision/stable/index.html
numpy: https://numpy.org
torchsummary: https://pypi.org/project/torchsummary/
huggingface-hub: https://pypi.org/project/huggingface-hub/
transformers: https://pypi.org/project/transformers/