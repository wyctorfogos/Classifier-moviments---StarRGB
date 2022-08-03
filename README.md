# Classifier-moviments---StarRGB
Train different models using Transfer Learning - 6 moviments


To use it, import the folders with your custom images running:

X = files.upload()
y = files.upload()

or load the numpy files:

import numpy as np

X = []
y = []

#for features,label in training_data:
#    X.append(features)
#    y.append(label)

X = np.load("/content/drive/MyDrive/REDES NEURAIS/DE IMAGENS/X_{}.npy".format(tipo_dos_dados))
y = np.load("/content/drive/MyDrive/REDES NEURAIS/DE IMAGENS/y_{}.npy".format(tipo_dos_dados))

