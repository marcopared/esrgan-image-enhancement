# Enhanced Super-Resolution GANs Project Report
For more information, please read Project_Report.pdf
## Authors
- Marco Paredes (Electrical and Computer Engineering, A15951023)

## Abstract

Enhanced Super-Resolution Generative Adversarial Networks (ESRGAN) are deep convolutional GAN networks used for image super-resolution. This project explores ESRGAN's ability to generate high-resolution images, implementing enhancements from the original SRGAN architecture. The results demonstrate that ESRGAN outperforms other models like RCAN, EDSR, and EnhanceNet. Three different datasets were examined, including one with degraded (noisy) images, to further understand the generator's performance.

## Introduction

ESRGAN's primary goal is to upscale low-resolution images while maintaining high-quality visual details. This project further analyzes the model by training three different models on datasets including celebrities, dog images, and degraded noisy pictures. The approach involves understanding and improving both the generator and discriminator's capabilities.

## Related Work

ESRGAN builds on SRGAN, introducing improvements that lead to more realistic generated images. Research has been further extended with Real-ESRGAN, designed to handle real-world, degraded images with enhanced perceptual quality.

## Method

The project implemented ESRGAN, detailing its structure and specific components in PyTorch. Key parts include the generator's total loss function and the model's innovative Residual in Residual Dense Blocks (RRDB).

![Discriminator and Generator Diagram](discriminator_and_generator.png)
![RRDB Diagram](rrdb.png)

## Experiments

Three different datasets were utilized:

1. **Celebrity Dataset**: Proved effective in producing higher-quality images.
2. **Dog Dataset**: Produced higher-quality images with added contrast and brightness.
3. **Noisy Dog Dataset**: The generator was not as effective with noisy images.

### Results

#### Celebrity Dataset
![Celebrity Images](img_align_celeba_images.jpg)
![Celebrity Training Results](img_align_celeba_training_results.jpg)

#### Dog Dataset
![Dog Images](img_dogs_images.jpg)
![Dog Training Results](img_dogs_training_results.jpg)

#### Noisy Dog Dataset
![Noisy Dog Images](img_noisy_dogs_images.jpg)
![Noisy Dog Training Results](img_noisy_dogs_training_results.jpg)

## Conclusion

The ESRGAN has shown to be effective in producing high-quality images from low-resolution inputs, even with minimal data and training. Future work could explore additional enhancements, test the model with other diverse datasets, and analyze its application in handling more real-world scenarios.
