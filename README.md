# DeepCarcinoma

The assigned original project focused on leveraging the fastai library, a Python deep learning framework built on PyTorch, for the classification of breast histopathology images. The Kaggle dataset utilized contained over 400,000 images categorized into class 0 (healthy tissues) and class 1 (diseased). To handle this data, loading procedures considered validation percentages, defined augmentation criteria, and established an ImageDataBunch. A transfer learning strategy was adopted, employing a pre-trained ResNet18 Convolutional Neural Network from the ImageNet database. Fine-tuning involved adjusting the weights of the last layers along with the learning rate parameter, resulting in an impressive 89% accuracy.

The project showcased the efficacy of transfer learning and data augmentation but faced limitations, including an outdated fastai library version, interpretability challenges due to Fastai's high-level abstractions, class distribution imbalance, and absence of a dedicated test set, raising concerns about model generalization.

To address these limitations, the current project endeavours to:

- Transition from fastai to Keras for building, training, and deploying the neural network.

- Mitigate class imbalance by introducing weights that prioritize accurate classification of class 1.

- Allocate 15% of the dataset for comprehensive testing, adjusting the training-evaluating-test set percentages to 70-15-15%.

- Explore the potential advantages of ResNet50 over ResNet18 and compare their performances with a transfer learning model built upon Efficient Net, as covered in theoretical lessons.
