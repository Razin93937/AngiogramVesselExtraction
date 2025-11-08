# AngiogramVesselExtraction

A MATLAB App Designer project for vessel enhancement, segmentation, and ridge extraction using multiscale filtering, eigenvalue-based vesselness, and MLSEC curvature analysis.

![GUI Screenshot](images/preprocessing.png)
![GUI Screenshot](images/segmentation.png)
*Screenshots of the App interface.*

---

## Features

### Preprocessing
- Median filtering  
- Multiscale tophat enhancement  
- Adaptive Histogram Equalization (CLAHE)  
- Unsharp masking  
- Guided filtering  

### Vesselness Detection
- Multiscale Frangi-inspired vesselness  
- Hessian eigenvalue analysis  
- Vesselness heatmap  
- Optional visualization on the original image  

### Morphological Segmentation
- Adaptive thresholding  
- Largest-area component filtering  
- Hole filling and refinement  
- Perimeter and mask overlays  

### Ridge Extraction
- Skeletonization via `bwmorph` or `bwskel`  
- MLSEC ridge detector  
- Ridge overlay in red  
- Binary ridge map export  

---

## Typical Workflow
- Load an image (retina fundus image recommended)
- Choose Preprocessing operations
- Compute Vesselness
- Adjust threshold
- Apply Morphological cleanup
- Extract Ridges
- Visualize overlays or export masks

## Citations

[1] Guo, D., & Richardson, P. D. (2002). Automatic vessel extraction from angiogram images. https://doi.org/10.1109/cic.1998.731897

[2] ‌Fazlali, H. R., Karimi, N., Soroushmehr, S. M. R., Shirani, S., Nallamothu, B. K., Ward, K. R., Samavi, S., & Najarian, K. (2018). Vessel segmentation and catheter detection in X-ray angiograms using superpixels. Medical & Biological Engineering & Computing, 56(9), 1515–1530. https://doi.org/10.1007/s11517-018-1793-4

[3] Tsai, Y.-C., Lee, H.-J., & Yu-Chih Chen, M. (2015). Automatic segmentation of vessels from angiogram sequences using adaptive feature transformation. Computers in Biology and Medicine, 62, 239–253. https://doi.org/10.1016/j.compbiomed.2015.04.029

[‌4] Lopez, A. M., Lumbreras, F., Serrat, J., & Villanueva, J. J. (1999). Evaluation of methods for ridge and valley detection. IEEE Transactions on Pattern Analysis and Machine Intelligence, 21(4), 327–335. https://doi.org/10.1109/34.761263

[‌5] Guo, N. D. (2002). Intravascular ultrasound speckle statistics. 2, 796–799. https://doi.org/10.1109/iembs.1998.745551




