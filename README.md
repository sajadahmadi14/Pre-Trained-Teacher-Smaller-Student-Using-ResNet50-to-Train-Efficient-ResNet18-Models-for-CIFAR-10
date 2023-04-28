# Pre-Trained-Teacher-Smaller-Student-Using-ResNet50-to-Train-Efficient-ResNet18-Models-for-CIFAR-10
Knowledge Distillation technique to train a smaller model using a larger pre-trained model. Here are the steps involved:

First, a ResNet50 model is prepared and pre-trained on the ImageNet dataset.
The final fully connected layer of the ResNet50 model is replaced with an appropriately sized layer for the CIFAR-10 problem.
Keeping the other parameters of the network constant, only the last layer is trained and evaluated on the CIFAR-10 dataset.
Using the pre-trained ResNet50 model as a teacher, a ResNet18 model is trained from scratch on CIFAR-10, using the Knowledge Distillation technique with α and τ tests.
In another task, a ResNet18 model is also trained and evaluated from scratch without using a pre-trained model.
The difference between the performance of the ResNet18 model trained using Knowledge Distillation and the ResNet18 model trained from scratch could be attributed to several factors.

When using the Knowledge Distillation technique, the pre-trained ResNet50 model acts as a teacher and transfers its knowledge to the ResNet18 model during training. Thus, the ResNet18 model benefits from the pre-trained model's experience and learns more efficiently. This can result in better generalization and improved accuracy compared to training the ResNet18 model from scratch.

On the other hand, when training the ResNet18 model from scratch, the model has to learn everything from the beginning without any prior knowledge transfer. This requires more data and computing resources and can take longer to achieve good performance. Therefore, the performance of the ResNet18 model trained from scratch may not be as good as the model trained using Knowledge Distillation.

Overall, the use of Knowledge Distillation can be an effective way to improve the performance of smaller models by leveraging the knowledge learned by a larger pre-trained model.
