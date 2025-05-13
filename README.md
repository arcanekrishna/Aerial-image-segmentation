# AERIAL IMAGE SEGMENTATION USING PyTorch
This project implements a deep learning model for segmenting roads in aerial images, using a U-Net architecture to predict binary masks (road vs. non-road regions).Designed with potential use in urban planning, autonomous driving, or geographic analysis.

# Model
Utilizes a U-Net model from segmentation_models_pytorch for road segmentation in aerial images.
Employs a timm-efficientnet-b0 encoder pretrained on ImageNet for robust feature extraction.
Outputs logits for binary segmentation (road vs. non-road), converted to probabilities via sigmoid.

# Loss function
Combines Dice Loss (optimizes overlap between predicted and ground truth masks) and Binary Cross-Entropy (BCE) Loss (measures pixel-wise probability errors).
Encourages accurate and smooth segmentation.
