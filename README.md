# Grading of Neyriz Marble and Natanz Granite Stones

This bachelor's thesis studied whether features extracted from stone photographs could distinguish two stone types across three quality grades each. The work was supervised by Dr. Marzieh Zarrinbal at Amirkabir University of Technology.

## Data and methods

The dataset contained 279 RGB images across six classes. A stratified split assigned 195 images to training, 42 to validation, and 42 to held-out testing. ImageNet-pretrained ResNet50, MobileNetV2, and EfficientNet-B0 served as fixed feature extractors. The resulting feature vectors were classified with k-nearest neighbors or random forest, giving six extractor–classifier combinations.

## Held-out results

| Feature extractor and classifier | Accuracy | Weighted F1 |
| --- | ---: | ---: |
| EfficientNet-B0 + Random Forest | 97.62% | 97.61% |
| MobileNetV2 + Random Forest | 97.62% | 97.58% |
| ResNet50 + Random Forest | 95.24% | 95.18% |
| EfficientNet-B0 + KNN | 95.24% | 95.17% |
| ResNet50 + KNN | 88.10% | 87.96% |
| MobileNetV2 + KNN | 85.71% | 85.25% |

The highest weighted F1 came from EfficientNet-B0 with Random Forest. Both leading combinations correctly classified 41 of 42 test images. These are the results reported in the thesis. The small test set and the focus on two stone types limit what can be inferred about other materials or imaging conditions.

The original source code and image dataset are currently unavailable for this portfolio. The thesis results have not been rerun.
