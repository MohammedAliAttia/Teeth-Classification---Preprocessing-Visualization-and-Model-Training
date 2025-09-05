# Teeth Classification Project - Baseline Report

## Project Overview
- **Objective**: Develop a CNN model for dental image classification
- **Classes**: 7 categories (OT, CoS, MC, CaS, OC, OLP, Gum)
- **Total Dataset**: 5,143 images

## Dataset Distribution
- **Training**: 3,087 images
- **Validation**: 1,028 images
- **Testing**: 1,028 images

## Baseline Performance
- **Overall Accuracy**: 0.676 (67.6%)
- **Macro F1-Score**: 0.672
- **Weighted F1-Score**: 0.677

## Class-wise Performance
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| OT | 0.660 | 0.725 | 0.691 | 131 |
| CoS | 0.676 | 0.671 | 0.673 | 149 |
| MC | 0.737 | 0.683 | 0.709 | 180 |
| CaS | 0.729 | 0.656 | 0.691 | 160 |
| OC | 0.580 | 0.704 | 0.636 | 108 |
| OLP | 0.744 | 0.661 | 0.700 | 180 |
| Gum | 0.575 | 0.642 | 0.606 | 120 |

## Key Findings
1. **Best Performing Classes**: MC and CaS show highest precision (>0.72)
2. **Challenging Classes**: OC and Gum need improvement (precision <0.60)
3. **Overall Assessment**: Baseline achieves 67.6% accuracy

## Next Steps & Recommendations
1. **Data Augmentation**: Implement more aggressive augmentation for underperforming classes
2. **Architecture Optimization**: Experiment with different CNN architectures
3. **Transfer Learning**: Consider pre-trained models (ResNet, EfficientNet)
4. **Class Balancing**: Address class imbalance in the dataset
5. **Hyperparameter Tuning**: Optimize learning rate, batch size, and regularization

## Files Generated
- `baseline_report.json`: Detailed metrics and confusion matrix
- `README.md`: This summary report
- Visualization plots showing performance metrics