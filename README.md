# Classifier-moviments---StarRGB
Train different models using Transfer Learning - 6 moviments


To use it, import the folders with your custom images running:

X = files.upload()
y = files.upload()

or load the numpy files:

import numpy as np

X = []
y = []

X = np.load("/content/drive/MyDrive/REDES NEURAIS/DE IMAGENS/X_{}.npy".format(tipo_dos_dados))
y = np.load("/content/drive/MyDrive/REDES NEURAIS/DE IMAGENS/y_{}.npy".format(tipo_dos_dados))

To enable the GPU, use the command below:

config = tf.compat.v1.ConfigProto(device_count = {'GPU': 80 , 'CPU': 60} )#device_count = {'GPU': 20 , 'CPU': 56} ) #intra_op_parallelism_threads=NUM_THREADS)# 
sess = tf.compat.v1.Session(config=config)#sess = tf.Session(config=tf.ConfigProto(gpu_options=gpu_options)) 
tf.compat.v1.keras.backend.set_session(sess)
