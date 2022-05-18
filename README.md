# Pre-trained Image Classifier to Identify Dog Breeds

An image classification application using a deep learning model called a convolutional neural network (often abbreviated as CNN) to identify dog breeds.

CNNs work particularly well for detecting features in images like colors, textures, and edges; then using these features to identify objects in the images. You'll use a CNN that has already learned the features from a giant dataset of 1.2 million images called ImageNet.

There are different types of CNNs that have different structures (architectures) that work better or worse depending on your criteria. With this application you can use the three different architectures (**AlexNet**, **VGG**, and **ResNet**) and determine which is best for your results.

### Used Tools
* [Python 3](https://www.python.org/downloads/)
* [Pillow](https://pillow.readthedocs.io/en/stable/installation.html)

### How to Run
1. Open your terminal.
2. cd to the application folder.
3. Run Python file called **check_images.py** using three arguments `--dir`, `--arch`, `--dogfile` and use `>` symbol, where:
    * `--dir`: Images Folder - _ex: pet_images_.
    * `--arch`: CNN Model Architecture - _ex: vgg_.
    * `--dogfile`: Text File with Dog Names - _ex: dognames.txt_.
    * `>`: Pipe to print output into a file.

##### Examples
```
python check_images.py --dir pet_images/ --arch resnet  --dogfile dognames.txt > resnet_pet-images.txt
python check_images.py --dir pet_images/ --arch alexnet --dogfile dognames.txt > alexnet_pet-images.txt
python check_images.py --dir pet_images/ --arch vgg  --dogfile dognames.txt > vgg_pet-images.txt
```

### Where to put dog images
After testing the sample images you can put your images instead of them in pet_images folder.

### Directions for used images
* Images are in jpeg format with extension jpg.
* Images are approximately square in shape (their height and width are approximately the same number of pixels).
* Dog Image - named Dog_01.jpg. This name is formatted such that if more than one word makes up the dog name those words are separated by an underbar ( _ ).
* For example:
    * Image of a Field Spaniel is named Field_Spaniel_01.jpg.
* Make sure you know the breed of dog that the image is of.