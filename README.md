# Benchmarking distributed tensorflow with affordable GPUs
We extend the benchmark [results](https://www.tensorflow.org/performance/benchmarks) published in Tensorflow official website to more afforable hardware platforms with consumer grade GPUs, i.e. GTX 1080 cards with PCI switches.  

A few image classification models are selected to add the reference points. The details of the [methodology](https://www.tensorflow.org/performance/benchmarks#methodology) is describled in the Tensorflow website.

## Test Environment
**Xpander Type**: CUBIX
**GPU**: 8x NVIDIA GTX 1080
**OS**: Ubuntu 16.04 LTS
**CUDA / cuDNN**: 8.0 / 5.1
**TensorFlow Version**: 1.1
**CPU**: 2x Intel Xeon E5-2620
**Disk**: Local SSD
**DataSet**: ImageNet
