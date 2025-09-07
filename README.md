# Replicating Vision Transformer (ViT) in PyTorch

This notebook replicates the Vision Transformer (ViT) as described in the paper "An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale" using PyTorch.

The notebook covers the following steps:

1.  **Setup**: Setting up the environment and downloading the necessary data (pizza, steak, sushi images).
2.  **Data Preparation**: Creating PyTorch Datasets and DataLoaders for the image data.
3.  **ViT Architecture Replication**: Step-by-step implementation of the core components of the ViT model:
    *   Patch Embedding: Converting images into sequences of patches and embedding them.
    *   Class Token and Position Embedding: Adding special tokens and positional information to the patch embeddings.
    *   Multihead Self-Attention (MSA) Block: Implementing the self-attention mechanism.
    *   Multilayer Perceptron (MLP) Block: Implementing the feed-forward network.
    *   Transformer Encoder: Combining MSA and MLP blocks to form the Transformer Encoder layer.
4.  **Building the ViT Model**: Assembling the custom ViT model using the implemented components.
5.  **Training Setup**: Setting up the optimizer and loss function for training the custom ViT model.
6.  **Training Custom ViT**: Training the custom ViT model on the prepared dataset.
7.  **Pretrained ViT**: Utilizing a pretrained ViT model from `torchvision.models` as a feature extractor.
8.  **Data Preparation for Pretrained ViT**: Preparing the data with appropriate transforms for the pretrained ViT.
9.  **Training Pretrained ViT**: Training the pretrained ViT feature extractor model.
10. **Saving the Model**: Saving the best performing pretrained ViT model.
11. **Custom Image Prediction**: Making predictions on a custom image using the trained pretrained ViT model.

Final Training Accuracy: 99.21%
Final Testing Accuracy: 91.76%
