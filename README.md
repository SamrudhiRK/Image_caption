# Image_caption
Building an image caption generator to load a random image and give some captions describing the image. We will use Convolutional Neural Network (CNN) for image feature extraction and Long Short-Term Memory Network (LSTM) for Natural Language Processing (NLP).

### About the model
- Uses vgg16 for feature extraction (connected with only the previous layer)
- Features stored in a pickle file.
- 90% of the data for training (as it is a smaller data set)
- 40% of neurons dumped to reduce over fitting
- BLEU Score is used to evaluate the predicted text against a reference text, in a list of tokens.


### Running the code
All the images are present in the images folder. The caption.csv file contains all the captions. The caption file, the image folder and the jupyter-notebook are in the same folder. If the data is in another folder, corrections can be made accordingly.
```
BASE_DIR = ''
WORKING_DIR = ''
```
### About the data set
- The data set I've used is smaller flickr data set with 1000 images due to limited computational power.
- The image name and the captions are seperated by ',' in this data set.

## Required Modules 
```
pip install numpy tqdm tensorflow
```

