# What pys for:
1. ImageFeatureDataGenerator.py: to obatain raw image vector.

2. ImageFeature.py: to obtain image guidance vector. Note that the method they used was kind of different from
what's been talked in the paper, where they let those raw image vector passed through a one-layer NN.

3. AttributeFeature.py: to obtain raw attribute vector and attribute guidance vector. Note that they directly used the 
word embeddings of te five predicted attributes of those images, and they didn't provide code showing how they 
obtain them, like saying in the paper (ResNet-101......)

4. TextFeature.py: to obtain raw text feature (hidden states in each time step) and text guidance vector, and applied
early fusion. They also directly used the word embedding of the text and didn't provide code showing how they
generate the word embeddings saying in the paper (GloVe.....)

5. FuseAllFeature.py: apply representation fusion and modality fusion

6. FinalClassifier.py: The final classification step: a 2-layer NN.

7. LoadData.py: create dataloader to load text, image, and attribute data

# How to run:
Just run "run.ipynb". You may just ignore "Colab: Connect Google Drive" part, and also play with "Test .py" part to check if all .py work well. Then run "Train & Test" part.

# Download image data and image feature data:
Image data: https://drive.google.com/drive/folders/1vtQgCvntxiq_lCjyoIjJCaHHuW2KNQWY?usp=sharing

image feature data: https://drive.google.com/drive/folders/1-1WIwX2yLQCTsIXpjhhs0Rz8ZFMG3j8i?usp=sharing
