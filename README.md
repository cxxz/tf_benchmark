# Benchmarking distributed tensorflow with affordable GPUs
We extend the benchmark [results](https://www.tensorflow.org/performance/benchmarks) published in Tensorflow official website to more afforable hardware platforms with consumer grade GPUs, i.e. GTX 1080 cards with PCI switches.  

A few image classification models are selected to add the reference points. The details of the [methodology](https://www.tensorflow.org/performance/benchmarks#methodology) is describled in the Tensorflow website.

## Test Environment
* **Xpander Type**: CUBIX
* **GPU**: 8x NVIDIA GTX 1080
* **OS**: Ubuntu 16.04 LTS
* **CUDA / cuDNN**: 8.0 / 5.1
* **TensorFlow Version**: 1.1
* **CPU**: 2x Intel Xeon E5-2620
* **Disk**: Local SSD
* **DataSet**: ImageNet

```	    
      GPU0 GPU1 GPU2 GPU3 GPU4 GPU5 GPU6 GPU7 CPU Affinity
GPU0	 X 	 PIX	PIX	 PIX	SOC	 SOC	SOC	 SOC	0-5,12-17
GPU1	PIX	  X 	PIX	 PIX	SOC	 SOC	SOC	 SOC	0-5,12-17
GPU2	PIX	 PIX	 X 	 PIX	SOC	 SOC	SOC	 SOC	0-5,12-17
GPU3	PIX	 PIX	PIX	  X 	SOC	 SOC	SOC	 SOC	0-5,12-17
GPU4	SOC	 SOC	SOC	 SOC	 X 	 PIX	PIX	 PIX	6-11,18-23
GPU5	SOC	 SOC	SOC	 SOC	PIX	  X 	PIX	 PIX	6-11,18-23
GPU6	SOC	 SOC	SOC	 SOC	PIX	 PIX	 X 	 PIX	6-11,18-23
GPU7	SOC	 SOC	SOC	 SOC	PIX	 PIX	PIX	  X 	6-11,18-23 
```
