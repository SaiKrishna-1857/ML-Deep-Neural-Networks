
# Deep Neural Network Compression

## Authors & Affiliation
- Sai Krishna Sangeetha
- Venkata Sai Kumar Ganesula
- Sricharan Maddena
- Aishwarya Sripati
- College of Engineering and Computer Science, University of Central Florida, Orlando, Florida 32816

## Abstract
The project discusses the challenges of computational and storage costs associated with Convolutional Neural Networks (CNNs). We proposed a novel CNN pruning criterion inspired by the interpretability of neural networks. The relevance scores of essential components, like weights or filters, are determined automatically using explainable AI concepts. The strategy is demonstrated on the VGG16 model with the CIFAR-100 dataset. The compressed model performs better than earlier criteria.

## Background
Traditional pruning methods produce sparse weight matrices, which are challenging to optimize on general-purpose hardware. Structured pruning methods, which involve the removal of complete channels, have been devised to harness the benefits of pruning on general-purpose devices.

## Methodology
- The approach utilizes unstructured pruning to remove redundant or unimportant connections.
- Structured pruning involves removing entire channels or filters.
- Fine-tuning is done to transfer strong learned representations to other domains.

## Implementation
- The input to the model includes a pre-trained model, sparsity ratios, dataset batches, weight prune ratios, and specific criteria for both unstructured global pruning and structured pruning.
- The output is a pruned model.
- The implementation is performed on the VGG-16 architecture.

## Results
- The pre-trained VGG-16 model achieved a test accuracy of 74.44% and a test loss of 1.055.
- After pruning and fine-tuning, the model achieved a test accuracy of 74.15% with a test loss of 1.1855.

## Conclusion & Future Work
The report showcases a method to derive a lightweight network from a fine-tuned network. The initial size of the model (527.802 MB) was reduced to 46.334 MB, achieving a compression of 91.2% with a minimal accuracy drop. Future works include implementing iterative pruning and exploring dynamic or post-training quantization on the obtained model.

## References
A detailed list of references is available in the report.

## Code Link
The implementation is available in the Jupyter notebook `Deep_Neural_Network_Compression.ipynb`.
