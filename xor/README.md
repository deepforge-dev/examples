# XOR example
This is one of the canonical examples used in deep learning. This has been adapted from the [torch example](https://github.com/torch/nn/blob/master/doc/training.md).

This example trains a neural network to predict the XOR operation on two numbers where the number is true if it is < 0 and false if it is > 0, ie:

```
-1, -2 => false
-1, 2 => true
1, 2 => true
```

This can be rewritten as 

```
-1, -2 => (> 0)
-1, 2 => (< 0)
1, 2 => (< 0)
```

As you can see this, happens to correspond to multiplication between the input numbers and then checking the sign for the "truthyness". This approach is used in this example.
