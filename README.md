# XCAT-GAN
XCAT-GAN for Synthesizing 3D Consistent Labeled Cardiac MR Images on Anatomically Variable XCAT Phantoms

Sina Amirrajab, Samaneh Abbasi-Sureshjani, Yasmina Al Khalil, Cristian Lorenz, Juergen Weese, Josien Pluim, Marcel Breeuwer

Accepted for 23rd International Conference on Medical Image Computing & Computer Assisted Intervention (Oral presentation) [MICCAI](https://www.miccai2020.org/en/) 2020 


## Paper [arXiv](https://arxiv.org/abs/2007.13408v2)

### **Aim**
To address the lack of properly annotated data by synthesizing anatomically meaningful, controllable, and variable CMR images suitable for medical data augmentation. 
### **Propose**
To create a virtual population of anatomically variable patients by leveraging XCAT phantoms and synthesize CMR images by learning modality-specific features through conditional GANs.
### **Framework**
1. (simulated XCAT, XCAT labels) pairs to train a multi-class U-net. 
2. (real images, segmentation) pairs to train a conditional GAN.
3. (synthetic XCAT, XCAT labels) to augment and replace the real images.
### **Results**
- 3D volumetric consistency is achieved by using more XCAT labels.
- *Data augmentation* with XCAT-GAN synthetic images improves the generalizability of the segmentation network.
- *Real data reduction* experiment suggests to reduce the amount of real data up to 20% while retaining the performance.

### Framework
<p align='center'>
  <img src='visuals\method.png' width='800'/>
</p>

### Example Results
<p align='center'>
  <img src='visuals\results.png' width='800'/>
</p>

- 4-class vs 8-class XCAT-GAN synthesis
<p align='center'>
  <img src='visuals\visualization.gif' width='600'/>
</p>

- Short axis view, end-diastolic phase and end-systolic phase
<p align='center'>
  <img src='visuals\SA_ED.gif' width='200'/> 
  <img src='visuals\SA_ES.gif' width='200'/>
</p>

