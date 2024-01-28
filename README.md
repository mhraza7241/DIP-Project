**Analysis of Histopathological Images**
**Models**
1. Semantic segmentation of an image between 12 classes (modelU_v1_77 : 77% acc, 77% F1,
32% Iou)
2. Classification of input image between 3 classes (modelC_v1_60 : 60% acc, 59% F1)
For the semantic segmentation, we have used a Unet model with 1,925,964 parameters whereas
the classification model has 502,083 parameters.
<img width="486" alt="image" src="https://github.com/mhraza7241/DIP-Project/assets/153302030/6cb7833d-08f8-4719-b93b-394dc1b686e9">

**Pre-Processing**

The queensland data used in the following code is processed by following steps
1. Images: Gamma Correction (6)
2. Masks: Pixels that did not classify as one of the 12 classes were converted to background
pixels and the resulting image is encoded as 255x255x1 images.
<img width="371" alt="image" src="https://github.com/mhraza7241/DIP-Project/assets/153302030/09387acc-eb57-4900-b0ea-e302b9cbf4a8">

**Outputs and Confusion matrix:**

<img width="401" alt="image" src="https://github.com/mhraza7241/DIP-Project/assets/153302030/828b620c-386a-4ab9-8b57-a3aab1898160">


