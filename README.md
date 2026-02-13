# Real-time Domain Adaptation for Semantic Segmentation

This project investigates domain adaptation techniques for real-time semantic segmentation in autonomous driving scenarios. The goal is to reduce the performance gap when training on synthetic data (GTA5) and evaluating on real-world data (Cityscapes).

We adopt BiSeNet as a lightweight real-time segmentation model and systematically study:

• Baseline training on Cityscapes  
• Domain shift between GTA5 and Cityscapes  
• Data augmentation strategies  
• Fourier Domain Adaptation (FDA)  
• Domain Adaptation via Cross-domain Mixing (DACS)  
• A proposed hybrid CrossEntropy + Dice loss to handle class imbalance  

The proposed hybrid loss improves segmentation performance on underrepresented classes without modifying the network architecture.

## Key Results

• Cityscapes-only training (upper bound): 54.08 mIoU  
• GTA5 → Cityscapes baseline: 15.41 mIoU  
• FDA adaptation: 26.98 mIoU  
• Hybrid loss extension (proposed): 28.23 mIoU  

## Contributions

• Full domain adaptation pipeline for real-time segmentation  
• Implementation of FDA and DACS methods  
• Proposed hybrid CE + Dice loss for class imbalance  
• Extensive per-class IoU evaluation  

## Applications

• Autonomous driving  
• Real-time scene understanding  
• Synthetic-to-real transfer learning  

