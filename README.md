# Image-Caption-App-using-Streamlit
Image Caption App using Streamlit
### What is Image Captioning?
As the name implies, image captioning is the task of taking/inputting an image to an AI model, and receiving a text caption describing/summarizing the contents of the image as its output. 

Image captioning models consist of 2 main components: a CNN (Convolutional Neural Network) encoder and a Language Model/RNN (some sort of NLP model that can produce text) decoder. The CNN encoder stores the important information about the inputted image, and the decoder will use that information to produce a text caption.

To train image captioning models, the most commonly used datasets are the `Flickr8k` dataset and the `MSCOCO` dataset.

The `Flickr8k` dataset consists of `8000` images — each with 5 different captions that can describe the image — and the `MSCOCO` dataset consists of `328000` images

####Encoder-Decoder Model Architecture
An Encoder-Decoder architecture consists of 2 components: a Convolutional Neural Network to encode the image (i.e. transform it into a rich embedding representation), and a Recurrent Neural Network (or an LSTM) that will take in as input this image, and be trained to sequentially decode the caption using a mechanism called Teacher Forcing. A good diagram of what this model looks like is below:
