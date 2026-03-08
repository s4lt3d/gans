# GANs: Generative Adversarial Networks

> Multiple Generative Adversarial Network implementations in PyTorch and TensorFlow, including Vanilla GANs and DCGANs trained on MNIST and CIFAR10.

---

## Screenshots / Examples

<img src=".images/dcgan_mnist.gif" width="275"> <img src=".images/dcgan_cifar.gif" width="275">

MNIST-like and CIFAR-like generated images from Deep Convolutional GANs.

---

## Overview

This repository contains implementations of various GAN architectures in both PyTorch and TensorFlow. See [this blog post](https://medium.com/ai-society/gans-from-scratch-1-a-deep-introduction-with-code-in-pytorch-and-tensorflow-cb03cdcdba0f) for a detailed introduction to Generative Networks.

---

## Vanilla GANs

Based on the original paper [Generative Adversarial Networks](https://arxiv.org/abs/1406.2661) by Goodfellow et al.

Trained on [MNIST dataset](http://yann.lecun.com/exdb/mnist/) to generate hand-written digits using 1D vector representations for 2D input images.

- [PyTorch Notebook](https://github.com/diegoalejogm/gans/blob/master/Vanilla%20GAN%20PyTorch.ipynb)
- [TensorFlow Notebook](https://github.com/diegoalejogm/gans/blob/master/Vanilla%20GAN%20TensorFlow.ipynb)

<img src=".images/vanilla_mnist_pt_raw.png" width="300"> <img src=".images/vanilla_mnist_pt.png" width="300">

*MNIST-like generated images before & after training.*

---

## DCGANs (Deep Convolutional GANs)

Based on [Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](https://arxiv.org/abs/1511.06434) by Radford et al.

Trained on [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html) and [MNIST](http://yann.lecun.com/exdb/mnist/) datasets using 3D image representations (height × width × colors).

- [TensorFlow CIFAR10 Notebook](https://github.com/diegoalejogm/gans/blob/master/DC-GAN%20TensorFlow.ipynb)
- [PyTorch CIFAR10 Notebook](https://github.com/diegoalejogm/gans/blob/master/DC-GAN%20PyTorch.ipynb)
- [PyTorch MNIST Notebook](https://github.com/diegoalejogm/gans/blob/master/DC-GAN%20PyTorch%20(MNIST).ipynb)

<img src=".images/dcgan_cifar_pt_raw.png" width="300"> <img src=".images/dcgan_cifar_pt.png" width="300">

*CIFAR-like generated images before & after training.*

---

## Requirements

```bash
pip install -r requirements.txt
```

Key dependencies:

- PyTorch 1.0+
- TensorFlow 2.0+
- NumPy
- Matplotlib

---

## Project Files

- `1. Vanilla GAN PyTorch.ipynb` — Vanilla GAN implementation (PyTorch, MNIST)
- `1. Vanilla GAN TensorFlow.ipynb` — Vanilla GAN implementation (TensorFlow, MNIST)
- `2. DC-GAN PyTorch.ipynb` — Deep Convolutional GAN (PyTorch, CIFAR10)
- `2. DC-GAN TensorFlow.ipynb` — Deep Convolutional GAN (TensorFlow, CIFAR10)
- `2. DC-GAN PyTorch-MNIST.ipynb` — DC-GAN variant trained on MNIST
- `Vanilla-GANs-pytorch.py` — Standalone PyTorch implementation
- `utils.py` — Utility functions for loading and processing data

---

## Learning Resources

- [Detailed Blog Post](https://medium.com/ai-society/gans-from-scratch-1-a-deep-introduction-with-code-in-pytorch-and-tensorflow-cb03cdcdba0f) — Comprehensive GAN introduction
- Original Papers:
  - [Generative Adversarial Networks](https://arxiv.org/abs/1406.2661) — Goodfellow et al.
  - [Unsupervised Representation Learning with DCGANs](https://arxiv.org/abs/1511.06434) — Radford et al.

---

## License

[MIT License](LICENSE)
