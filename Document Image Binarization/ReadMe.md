# Document Image Binarization
This project was done under the guidance of [Prof J Jennifer Ranjani](https://www.bits-pilani.ac.in/pilani/jenniferranjani/profile)
Binarization refers to the conversion of a grayscale image into a Black and white image. In this project we wish to convert a convert an image of a document into the Binarized form.
This can be modelled as an image segmentation problem where we want to classify each pixel as either text or background. We first convert the document image to grayscale and then 
pass it through our network to segment out the text from the background. 
Our architecture is similar to the [Unet](https://arxiv.org/abs/1505.04597). The network is trained on a dataset made up of images from [Dibco](https://vc.ee.duth.gr/dibco2019/) using 
the Binary Crossentropy loss function.
We trained another network with the similar architecture but instead of normal convolutions, we used [Deformable Convolutions](https://arxiv.org/abs/1703.06211) which are able to handle
geometric variations or transformations better which resulted in a slight increase in the accuracy.
