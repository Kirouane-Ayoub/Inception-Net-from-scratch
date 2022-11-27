# Inception-Net-from-scratch : 



![1668369195022](https://user-images.githubusercontent.com/99510125/204151663-4a754c64-ef2c-4f2a-a921-07393d4eb23b.jpeg)

When multiple deep layers of convolutions were used in a model it resulted in the overfitting of the data. To avoid this from happening the Inception-V1 model uses the idea of using multiple filters of different sizes on the same level. Thus in the inception models instead of having deep layers, we have parallel layers thus making our model wider rather than making it deeper.


![1667986896584](https://user-images.githubusercontent.com/99510125/204151698-99612657-3cc6-43e8-b5cd-c44497f497e1.jpeg)


The above-depicted Inception module simultaneously performs 1 * 1 convolutions, 3 * 3 convolutions, 5 * 5 convolutions, and 3 * 3 max pooling operations.
Thereafter, it sums up the outputs from all the operations in a single place and builds the next feature. The architecture does not follow the Sequential model approach where every operation such as pooling or convolution is performed one after the other.

The Inception module with dimension reduction works in a similar manner as the naïve one with only one difference. Here features are extracted on a pixel level using 1 * 1 convolutions before the 3 * 3 convolutions and 5 * 5 convolutions. When the 1 * 1 convolution operation has been performed the dimension of the image is not changed. However, the output achieved offers better accuracy.

For more information visit : https://www.linkedin.com/pulse/going-deeper-convolutions-inception-googlenet-ayoub-kirouane
