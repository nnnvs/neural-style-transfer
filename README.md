# neural-style-transfer

Please find project_report.pdf which investigates various techniques for style transfer using deep learning from the method described by Gatys to CycleGANs.

![Example Image](img/example.png)

Neural Style Transfer utilizes the [VGG-19 Image Classification Neural Network](https://arxiv.org/pdf/1409.1556.pdf) to apply transfer learning to images. 

![VGG19 - Clifford K. Yang](https://github.com/27pirateking/neural-style-transfer/blob/master/img/vgg19.jpg?raw=1)

This repository explores two methods - one introduced by Leon A. Gatys, and another introduced by Justin Johnson.

[Gatys' method](https://arxiv.org/pdf/1508.06576.pdf) is an iterative process (typically 150-200 iterations) to optimize a generated image, based on a cost function for style and content. The content cost function is defined by comparing the outputs of `conv4_2` between the generated image and the content image. The style cost function is defined by comparing the outputs of `[conv1_1, conv2_1, conv3_1, conv4_1, conv5_1]` between the generated image and the style image.

The main notebook, Neural_Style_Transfer.ipynb, contains all relevant documentation for this repository.