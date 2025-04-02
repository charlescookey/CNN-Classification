# CNN Classification

Small object detection is a critical and challenging task for perception systems. 
The purpose of this CNN model to detect objects from the dataset.

## Architecture

* Input, The image would be transformed to grey scale. Hence, in_channels is set to 1.
* Conolutional Layer 1: This layer is to extract a basic features from the image like texture and edges and simple patter. A kernel size of 5x5. This would allow it capture global patterns. A stride of 1 is used to allow for overlapping of receptive field, hence capturing more detial.
* Pooling layer 2: This layer is used to reduce spatial dimesion while retaiinig the importand information. A stride of 2 was used, this would help avoid overfitting, as it would reduce the overlapping of recpetive fields.
* Convolution Layer 3: This layer is to extract more complex patters and shapes. A kernel size of 5x5 was also used, and a stride of 1
* Pooling layer 4: Similar to 2, we also want to futher reduce the feature mapo size and reove less significant details
* Convolution Layer 5: this layer us to extract the higher level features that are needed for calssification
* Fully connected layer 6: The feature maps is converted into a vector for the classification preocess
* Fully connected layer 7.
* Fully connected layer 8.

  
## Improvements
* Methods used to deal with varying input sizes
  * Resising input size
  * Padding
  * Global Average Pooling
  * Global Max Pooling
* Using different optimizer
* Learning rate scheduling
* Data augumentation
