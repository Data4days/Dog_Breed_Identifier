# Dog_Breed_Identifier

This project aims to implement algorithms to identify whether a presented image contains humans or dogs. If there is a dog in the image, the goal is to identify the breed of the dog with acceptable accuracy. If there is a human in the image, the algorithm gives the dog breed which the human most closely resembles.

[Haar feature-based cascade classifiers](http://docs.opencv.org/trunk/d7/d8b/tutorial_py_face_detection.html) were used to identify if the images contained human faces.

I then built a convolutional neural network from scratch to identify the dogs and dog breeds. This model produced an accuracy of 8.61%. Given that there are 133 dog breeds present in the training files, a random guess has a 1/133 (0.8%) chance of being right. The CNN is therefore significantly more accurate than random guessing.

For my next step, I built a CNN using transfer learning with the [Xception](https://arxiv.org/abs/1610.02357) architecture. This model achieved an accuracy of 85.17%.

Lastly, 5 test images were uploaded with the results shown in the notebook.
