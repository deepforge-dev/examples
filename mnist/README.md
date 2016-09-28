# MNIST
An example which trains a classifier on the [MNIST](http://yann.lecun.com/exdb/mnist/) data set. 

This example uses [torchnet](https://github.com/torchnet/torchnet) to showcase the flexibility of both DeepForge and torchnet by extending their [example code](https://github.com/torchnet/torchnet/blob/master/example/mnist.lua).

# Installation
Assuming torch is already installed, torchnet can easily be installed with *luarocks* 
```
luarocks install torchnet
```

To run this example you must also have the `mnist` package as well:
```
luarocks install mnist
```
