# image-captioning-generator

Image caption generator is a process of recognizing the context of an image and annotating it with relevant captions using deep learning and computer vision. It includes labeling an image with English keywords with the help of datasets provided during model training. The imagenet dataset trains the CNN model called Resnet. Resnet is responsible for image feature extraction. These extracted features will be fed to the T5 model, which generates the image caption.

encoder:
CNN – To extract features from the image. A pre-trained model called Resnet is used for this.
decoder:
T5 – To generate a description from the extracted information of the image.


Model performance was evaluated using BLEU score. These results (quantitative and qualitative) were acquired by leveraging greedy decoding. Results of higher quality can be obtained by using beam search which isn't implemented in this repo.
