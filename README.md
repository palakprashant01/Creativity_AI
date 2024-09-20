# Purpose of the Project:
1. Utilize AI for generating innovative art.
2. Grasp the principles of the DeepDream algorithm.
3. Build, train, and evaluate the DeepDream algorithm for producing art with AI, using the Keras API and TensorFlow 2.0.
4. Use the DeepDream algorithm to add psychedelic effects to images and videos.
5. Comprehend gradient ascent and the maximization of activations.
6. Explore the Inception Net deep neural network model developed by Google.

Creative AI is a new branch within AI wherein it can create paintings, produce new music, write stories. In this project, we will apply AI to generate art for us. We will use the Deep Dream algorithm to create almost creepy/trippy images. We will also understand what the model views/what truly happens within the hidden layers in the model to generate art.

When we try to run the Deep Dream algorithm, we try to maximize the activations or what the hidden layers can see.

1. Deep Dream is an algorithm created by Google that produces images with a surreal, dream-like quality, reminiscent of the effects of potent hallucinogens.
2. The algorithm is trained on millions of images to enhance and create increasingly unusual features.
3. It amplifies the patterns within an image based on its prior training, emphasizing elements it recognizes.
4. For instance, if the algorithm has learned to identify airplanes, it will attempt to highlight airplane-like characteristics in any given image.

# Understanding the Deep Dream Algorithm:
1. If we take an image and feed it to a pre-trained convolutional neural network, we will find that the first layers generally capture low-level features, called edges/curves.
2. As we go deeper in the network, we will find that higher level features are detected, like faces and cars.
3. The final few layers very deep into the model assemble into complete inferences. These neurons are generally activated in response to complex things such as buildings, etc.
4. The kind of layers we select will impact the response of the network. <br />

How does the deep dream algorithm work?
1. If we have a pre-trained network and an input image and we pass this image to the network, a series of activations will be generated.
2. We want to take these activations and manipulate the input image in a way to maximize the activations coming from the corresponding layers.
3. So, if we ask the first couple of layers and the last couple of layers to maximize what they see/detect, a phenomeon called "inceptionism" occurs, wherein the results become dreamy.
4. So, the model superimposes what it has already been trained to see on the original image, churning out trippy images.
5. So, when we feed an image to a trained artificial neural network, the neurons fire and generate activation. The model tries to change the input image so that some of these neurons can fire more and maximize activations (we can select which particular neurons in which specific layers should fire more as well).
6. This process is repeated continuously until the input image contains the features the layer was initially looking for (for example, detecting cats in a pink sky until the model starts creating cat faces on top of the pink sky, until the layer is satisfied with the results). <br />

The following are the specific steps of the deep dream algorithm:
1. Feed an image through a pre-trained artificial neural network or convolutional neural network or a residual neural network or inception net neural network, or any other appropriate neural network.
2. Then, we will select a layer (the initial layers capture lines/edges/basic shapes, while the deep layers capture full shapes, like faces, buildings, and animals).
3. Calculate the activations generating from the selected layer.
4. Calculate the activation gradient with respect to the input image fed to the network.
5. Modify the image until the activations are maximized, increasng the patterns seen by the network.
6. Repeat steps 1-5 across multiple scales.

# Note:
Since the Colab notebook was too large a file, a PDF file has been attached. Several images of the outputs have been hidden or deleted to accomodate the upload to GitHub.
