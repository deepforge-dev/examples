# Galaxy Zoo Example
This is a simple example using the Galaxy Zoo dataset (also seen in [the Galaxy Challenge](https://www.kaggle.com/c/galaxy-zoo-the-galaxy-challenge) on [kaggle](www.kaggle.com)). This example also demonstrates how a large dataset can be imported into DeepForge and streamed to the neural network during training.

The example project contains the training data and can be downloaded from [here](https://deepforge.s3.amazonaws.com/galaxy-data.webgmex?AWSAccessKeyId=AKIAISTYNTKQZLV6IVLQ&Expires=1633932738&Signature=8%2BlF1x%2FsF0fGE0K0DGBLjG1R9v0%3D). Or, if you prefer downloading from the console:

```
wget -O galaxy-data.webgmex https://deepforge.s3.amazonaws.com/galaxy-data.webgmex?AWSAccessKeyId=AKIAISTYNTKQZLV6IVLQ&Expires=1633932738&Signature=8%2BlF1x%2FsF0fGE0K0DGBLjG1R9v0%3D
```

In this example, we are simply cropping a 106x106 section of the image and training either a feed-forward neural network or a convolutional neural network. The architecture for the convolutional neural network is based on the paper by Sandor Dieleman. The entire citation for the paper is given below.

```
@article{dieleman2015rotation,
  title={Rotation-invariant convolutional neural networks for galaxy morphology prediction},
  author={Dieleman, Sander and Willett, Kyle W and Dambre, Joni},
  journal={Monthly notices of the royal astronomical society},
  volume={450},
  number={2},
  pages={1441--1459},
  year={2015},
  publisher={Oxford University Press}
}
```

This example depends on the [deepforge-keras](https://github.com/deepforge-dev/deepforge-keras) extension.
