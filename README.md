CUDA Denoiser For CUDA Path Tracer
==================================

**University of Pennsylvania, CIS 565: GPU Programming and Architecture, Project 4**

* Saksham Nagpal  
  * [LinkedIn](https://www.linkedin.com/in/nagpalsaksham/)
* Tested on: Windows 11 Home, AMD Ryzen 7 6800H Radeon @ 3.2GHz 16GB, NVIDIA GeForce RTX 3050 Ti Laptop GPU 4096MB

## Summary
TODO

## Representative Outcomes  
TODO

# Visual Parity Analysis

## Are the results 'Visually Acceptable'?

| Pathtraced, 1000 iterations | Denoised, 100 iterations |  Difference |
|:--:|:--:|:--:|
| ![](images/cornell.2023-10-20_10-50-16z.1001samp.png) | ![](images/cornell.2023-10-20_10-50-16z.118samp_denoised.png) | ![](images/specular_compare_100denoised_vs_1knorm.png) |
| ![](images/cornell.2023-10-20_11-07-34z.1001samp.png) | ![](images/cornell.2023-10-20_11-07-34z.94samp_denoised.png) | ![](images/filter_100iters_base.png.png) |
| ![](images/cornell.2023-10-20_11-14-59z.5000samp.png) | ![](images/cornell.2023-10-20_11-14-00z.94samp_denoised.png) | ![](images/refractive_100denoised_vs_5knorm.png) |

| Pathtraced, 5000 iterations | Denoised, 500 iterations |  Difference |
|:--:|:--:|:--:|
| ![](images/cornell.2023-10-20_11-25-52z.5000samp.png) | ![](images/cornell.2023-10-20_11-21-45z.503samp_denoised.png) | ![](images/multi_500denoised_5knorm.png) |

## Effect of Filter Size

| Filter Size | Resulting Render | Observation |
|:--:|:--:|:--:|
| None (Pathtraced) | <img src="images/filter_100iters_base.png" width=500> | With just 100 iterations, our render is pretty noisy at the moment.<br>This scene notable has albedo mapping and a refractive material, the effects of denoising on which would be interesting to note. |
| 8X8 | <img src="images/filter_100iters_filteriter2.png" width=350> | TODO |
| 16X16 | <img src="images/filter_100iters_filteriter3.png" width=350> | TODO |
| 32X32 | <img src="images/filter_100iters_filteriter4.png" width=350> | TODO |
| 64X64 | <img src="images/filter_100iters_filteriter5.png" width=350> | TODO |
| 2048X2048 | <img src="images/filter_100iters_filteriter10.png" width=350> | TODO |

