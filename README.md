# FashionMNIST-CNN-PyTorch
Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes.
Three different models for the FashionMNIST dataset and compared their performance in terms of accuracy and other metrics. Additionally, plotted the confusion matrix for the best-performing model to gain further insights into its performance.

#### Getting Started
1. Clone the Repository
2. Install Dependencies : `pip install -r requirement.txt`
3. Open the jupyter lab : `jupyter lab`

###### Note : The models presented in this project were trained on a small number of epochs for demonstration purposes. You can experiment with different hyperparameters, such as learning rate, batch size, and number of epochs, to further improve the model's performance. By tweaking these parameters and potentially utilizing more advanced architectures, may achieve better results in terms of both loss and accuracy. Feel free to explore and modify the code to suit your specific needs and objectives

### Model Performance

| model_name         | model_loss | model_acc | train_time | train_device |
|--------------------|------------|-----------|------------|--------------|
| FashionMNISTModelV0 | 0.4766     | 83.43     | 37.569s    | cpu          |
| FashionMNISTModelV1 | 0.6850     | 75.02     | 39.885s    | cpu          |
| FashionMNISTModelV2 | 0.3218     | 88.30     | 38.987s    | cuda         |


### Confusion Matrix
Generated a confusion matrix for FashionMNISTModelV2, the best-performing model, to better understand its classification performance. The confusion matrix provides insights into how well the model is classifying different classes within the dataset.
###### Classes

| T-shirt/top | Trouser | Pullover | Dress | Coat |
|-------------|---------|----------|-------|------|
| Sandal      | Shirt   | Sneaker  | Bag   | Ankle boot |


<div style="text-align:center">
    <img src="https://github.com/sOR-o/FashionMNIST-CNN-PyTorch/blob/main/assets/confusionMatrix.png" height="600" width="600">
</div>

### Confusion Matrix Insights

- **Overall Performance**: The main diagonal contains high values, indicating effective classification across most classes.
- **Misclassifications**: Off-diagonal elements show instances of misclassification. For example, T-shirt/top instances are occasionally misclassified as shirts or pullovers.
- **Confusion between Similar Classes**: Similar classes like T-shirt/top, Shirt, and Pullover may be confused due to their visual similarities.
- **Performance Variation**: Some classes, like Ankle boot and Sneaker, have high accuracy, while others, like Shirt and Pullover, exhibit more frequent misclassifications.
- **Potential Improvements**: Strategies to reduce misclassifications between similar classes and improve overall model performance can be explored.



-Can be improved by transfer learning (obviously 😉)

## Contributing

Contributions to this project are welcome! Whether it's bug fixes, new features, or documentation improvements, your contributions are valuable.
