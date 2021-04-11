# MIDASLab Task-2
The Task 2 was concerned with our knowledge on Convolutional Neutral Networks. Its basic structure, playing with dataset and hyperparameters that make up the CNN's body.
The dataset given in the Part-1 was a subset of EMNIST which in extension to the Handwritten digits also contained alphabets in both lower and upper case bringing the total number of classes to 62 with exactly 40 images for each class.
Total size of dataset = 40*62 = 2480

In Part-1, a CNN model (model1 in code) was made from scratch. After lot of compiling and hyper parameter tuning, it was decided that the network doesn't need to be too deep to get a good accuracy. 
In fact, the depth only reduced the accuracy significantly.
Ultimately, the CNN model got an validation accuracy of about 70 % which is pretty neat for such a small dataset.

In Part-2, we had to use a pre-trained model (transfer learning) which could be any network (VGG19, AlexNet, GoogLeNet, ResNet and so on) to be trained on the famous MNIST dataset which is a subset of the EMNIST containing only images of handwritten 0 to 9 consisting of 60,000 training images and 10,000 testing images. Although this looks like a large dataset in comparison to the first, but it is still a smaller one in the deep learning community.

Also, after training on the pre-trained model (which I selected as VGG19, model2 in code), I compared its performance witha randomly initialzed network. For that, I selected the same which I trained from scratch in the Part-1 (model3 in code)

The performance was very much comparable of both the networks gettin a validation accuracy in excess of 99 % in both the cases. Since MNIST is a very simple dataset not having complex patterns to recognize, this is understandable.

Coming to the Part-3 wherein another dataset was given but here, the dataset was very complicated. The dataset given is not well understood. Since the parent folder has subfolders labelled as 0 to 9 for the respective classes, but the images inside the subfolders have random images of any digit from 0-9 (6000 approx in every subfolder), it is impossible to train the dataset with wrong labels. https://www.dropbox.com/s/otc12z2w7f7xm8z/mnistTask3.zip?dl=0
