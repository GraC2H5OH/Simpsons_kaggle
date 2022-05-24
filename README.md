# Simpsons_kaggle
If you want to do something with model, you need to download dataset and model weights -->
You can download dataset from Kaggle and model weighs from link bellow
# https://drive.google.com/file/d/1nfAx_g_vw2S4twouqG99_7or7ztl8dom/view?usp=sharing
If you want to use this model for testing on random picture from google, you shouldn't test model in screenshoots from simpsons because model was trained on simpsons screenshots. It's better to use pictures like that:
# ![example](https://static-sl.insales.ru/images/products/1/5019/436573083/medium_9.jpg)
# How to understand prediction
After downloading dataset, model weights and test picture, you should download pretrained resnet152 and load weights into model, then ise transformations_predict function with path to picture and trained model. After that you'll get tensor['n'] where n is class number, open train/simspsons_dataset directory and start counting folders from 0 to n, and n folder name it's prediction
