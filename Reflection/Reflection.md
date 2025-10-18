Reflective Report on CIFAR-10 Image Classification Project
Introduction

This reflection discusses my experiences and learning throughout the module on machine learning, focusing on my final project with the CIFAR-10 dataset. The objective was to design a convolutional neural network (CNN) from scratch and enhance its performance using VGG16-based transfer learning. The reflection uses Rolfe et al.’s (2001) framework (WHAT, SO WHAT, NOW WHAT) to evaluate my experiences, outcomes, and professional growth. It also acknowledges the unique challenges I faced, including missing Project 1 due to a medical surgery.

WHAT: Project Description and Outcomes

Due to ear surgery from 28 August until 16 October 2025, I was unable to participate in Project 1 and had limited interaction with group activities. As a result, this reflection and the project work represent my individual efforts rather than collaborative contributions.

The project began with data preparation and exploration. I imported the CIFAR-10 dataset, normalized pixel values, split the data into training, validation, and test subsets, and reviewed class distributions. Visualizations and descriptive statistics ensured the dataset was balanced, clean, and suitable for model training.

In Phase 2, I developed a CNN consisting of three convolutional layers, batch normalization, max-pooling, and fully connected layers, with dropout to prevent overfitting. The model was compiled using Adam optimizer and sparse categorical cross-entropy. Training with data augmentation over 10 epochs resulted in a training accuracy of 67.8%, validation accuracy of 69.8%, and a test accuracy of 70.06%. Analysis of the confusion matrix and classification report showed high performance across most classes, though distinguishing cats and dogs remained challenging.

Phase 4 involved transfer learning using VGG16. I added custom layers—global average pooling, dense layers with ReLU, and dropout—while freezing the base VGG16 initially. After training these layers, I fine-tuned the top four convolutional layers with a lower learning rate. This process produced a final test accuracy of 67.8%, smoother convergence, and minimal overfitting. Data augmentation and dropout improved generalization and training stability.

SO WHAT: Analysis and Reflection

Engaging in this project was both intellectually stimulating and emotionally challenging. Missing Project 1 due to surgery initially caused anxiety about catching up, understanding the content, and performing independently. I had to quickly adapt to working entirely alone, which required self-discipline, time management, and problem-solving.

Despite these challenges, the project helped me gain a deeper appreciation for data preprocessing. Normalization, proper dataset splitting, and class balancing significantly impacted model performance. I learned that the effectiveness of a neural network relies heavily on high-quality, clean, and well-prepared input data.

Building the CNN from scratch highlighted the trade-offs between model complexity, training time, and generalization. Although the CNN achieved reasonable accuracy, it struggled with visually similar classes, reinforcing that pre-trained architectures, like VGG16, can significantly improve results.

Implementing VGG16 transfer learning was particularly instructive. Leveraging pre-trained features accelerated training and improved generalization. Fine-tuning the top layers taught me about careful learning rate management and selective layer unfreezing. These techniques minimized overfitting and produced a more stable model.

Emotionally, I experienced frustration when validation accuracy plateaued or when misclassifications occurred. Working alone intensified these feelings but also encouraged critical self-reflection and independent problem-solving. Observing final metrics and smooth convergence provided a sense of achievement and reinforced my persistence and resilience.

The lack of team collaboration meant I relied solely on my initiative and self-motivation. While I missed the benefits of peer feedback, I also developed stronger self-directed learning skills and a deeper understanding of each stage of the machine learning workflow.

NOW WHAT: Learning Outcomes and Future Applications

This project has significantly strengthened my technical and professional capabilities. I enhanced my skills in Python, TensorFlow, and Keras and gained practical experience in CNNs, transfer learning, data augmentation, batch normalization, and dropout.

Reflecting on my independent experience highlighted the value of self-management and resilience. I learned how to recover from absence, manage my own pace, and still achieve meaningful outcomes in complex projects. I also recognized the importance of structured documentation, clear workflow organization, and iterative debugging, which will benefit future independent or team-based projects.

The project reinforced ethical and professional considerations, such as addressing dataset biases, ensuring balanced class representation, and interpreting results responsibly. In future projects, I plan to explore larger datasets, more advanced architectures like ResNet or EfficientNet, and model explainability techniques to improve both performance and interpretability.

Ultimately, this reflective exercise emphasized the importance of adaptability. Despite missing group collaboration and a key early project, I successfully completed an advanced machine learning project independently, demonstrating technical competence, critical reflection, and professional growth.

Conclusion

The CIFAR-10 project has been a transformative learning experience. Designing a CNN and extending it through VGG16 transfer learning developed my technical skills, reflective thinking, and resilience. While missing Project 1 and working independently presented challenges, these circumstances strengthened my self-directed learning, problem-solving abilities, and understanding of machine learning workflows.

This reflection illustrates that even under personal constraints, it is possible to achieve meaningful outcomes, apply theoretical knowledge in practice, and develop both technical and professional skills essential for a career in AI and machine learning.

References (Harvard Style)

Chollet, F. (2018) Deep Learning with Python. Shelter Island, NY: Manning Publications.

Krizhevsky, A., Hinton, G. and University of Toronto (2009) Learning multiple layers of features from tiny images. [Online] Available at: https://www.cs.toronto.edu/~kriz/cifar.html
 [Accessed 13 October 2025].

Simonyan, K. and Zisserman, A. (2015) Very Deep Convolutional Networks for Large-Scale Image Recognition. [Online] Available at: https://arxiv.org/abs/1409.1556
 [Accessed 13 October 2025].

TensorFlow (2025) Keras API Documentation. [Online] Available at: https://www.tensorflow.org/guide/keras
 [Accessed 13 October 2025].

Rolfe, G., Freshwater, D. and Jasper, M. (2001) Critical reflection in nursing and the helping professions: a user’s guide. Basingstoke: Palgrave Macmillan.

The University of Edinburgh (no date) Reflection Toolkit. [Online] Available at: https://www.ed.ac.uk/reflection-toolkit
 [Accessed 13 October 2025].
