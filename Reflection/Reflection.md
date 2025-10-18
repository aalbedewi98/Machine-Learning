# Reflective Paper on Machine Learning Project

## Introduction

During this module, I engaged with a range of machine learning concepts, including convolutional neural networks (CNNs), transfer learning, and data augmentation techniques, applying these skills to the CIFAR-10 dataset. While the module emphasized collaborative work, I was unable to participate in group activities due to a medical issue. I underwent ear surgery from 28 August until 16 October 2025, which caused me to miss the first project and significantly limited my ability to work with peers. As a result, I completed all assignments and the final project independently. Despite these challenges, the experience provided valuable learning opportunities, allowing me to develop resilience, self-discipline, and technical competence in a condensed timeframe [Rolfe, Freshwater and Jasper, 2001].

## WHAT: Project Experience

The project focused on building and evaluating a CNN for image classification on the CIFAR-10 dataset, followed by a fine-tuning phase using a VGG16-based transfer learning model. Phase 1 involved data preparation and exploration, where I loaded, normalized, and visualized the dataset, split it into training, validation, and test sets, and calculated descriptive statistics such as mean and standard deviation per color channel. Phase 2 focused on building a CNN from scratch, comprising three convolutional layers with batch normalization and max-pooling, followed by dense layers and dropout to prevent overfitting [Chollet, 2018].

Phase 3 involved training and evaluating the CNN using real-time data augmentation, including rotations, horizontal flips, and shifts. I monitored training and validation accuracy and loss across multiple epochs, analyzed the confusion matrix, and generated a classification report to assess precision, recall, and F1-scores for each class. Phase 4 implemented transfer learning using VGG16. Initially, I froze the base layers and trained the added dense layers, followed by fine-tuning the top four convolutional layers. The final model achieved test accuracy between 58% and 67.8%, demonstrating strong generalization to unseen data [Simonyan and Zisserman, 2015].

Completing these phases independently was challenging. Without peer support, I had to manage all aspects of the project, from coding to debugging to evaluation. I often felt lost when encountering errors or conceptual gaps, particularly during fine-tuning with VGG16. However, this provided a unique opportunity to critically analyze my work, troubleshoot independently, and consolidate my understanding of machine learning concepts.

## SO WHAT: Analysis of Learning

The experience of working independently highlighted both my strengths and areas for growth. Emotionally, it was difficult to navigate the project alone, and I experienced moments of frustration and uncertainty. Missing the first project initially made me feel behind, and I had to catch up in a limited timeframe. These challenges forced me to prioritize tasks, manage my time effectively, and maintain focus under pressure. I learned to break complex problems into smaller, manageable steps, improving my problem-solving skills and increasing my confidence in working independently [University of Edinburgh, no date].

Technically, I developed proficiency in Python and Keras, particularly in implementing CNNs, data augmentation, and transfer learning. I gained experience with hyperparameter tuning, batch normalization, dropout regularization, and evaluation metrics such as accuracy, precision, recall, and F1-score. Working solo meant I had to research solutions, read documentation, and experiment with different approaches without immediate peer feedback. This process enhanced my ability to learn autonomously, interpret model outputs critically, and reflect on the effectiveness of different techniques [Goodfellow, Bengio and Courville, 2016].

Additionally, this experience reinforced my understanding of professional and ethical considerations in machine learning. While I did not work in a team, I remained mindful of academic integrity by referencing sources appropriately and ensuring my work was original. I became more aware of how proper documentation, methodical experimentation, and transparent reporting contribute to the credibility and reliability of machine learning outcomes [Rolfe, Freshwater and Jasper, 2001].

## NOW WHAT: Application and Future Development

Reflecting on this module, I recognize several ways in which this experience will influence my future learning and professional development. First, working independently improved my resilience and self-directed learning skills, which will be valuable in both academic and workplace contexts. I now have greater confidence in tackling new datasets and machine learning problems without immediate guidance.

Second, the project has strengthened my technical competence, particularly in deep learning and transfer learning. These skills are directly applicable to future research or professional roles in AI and computer engineering. Understanding CNN architectures, feature extraction, and fine-tuning strategies equips me to handle complex real-world problems, such as image recognition tasks in autonomous systems, robotics, or healthcare applications.

Third, while I did not participate in team-based activities, the experience made me appreciate the benefits of collaboration. In future projects, I aim to combine the autonomy I developed during this module with effective teamwork. I now understand the value of sharing knowledge, peer feedback, and collaborative problem-solving, and I will actively contribute to team discussions and tasks in subsequent modules or professional settings [University of Edinburgh, no date].

Finally, this reflective process has emphasized the importance of continuous improvement. By critically evaluating my work, analyzing errors, and reviewing model performance, I have learned to adopt a structured approach to self-assessment. This habit will help me refine my technical skills, adapt to new challenges, and maintain high standards of professional and ethical practice in machine learning projects.

## Conclusion

In conclusion, completing this module independently due to medical circumstances was both challenging and rewarding. Missing the first project initially caused me to feel lost, but the experience accelerated my learning in a short period. I gained significant technical skills in CNNs, transfer learning, and data augmentation, while also developing resilience, self-directed learning abilities, and reflective practices. Although I missed the collaborative aspects of the module, I recognize the importance of teamwork and will integrate these lessons into future projects. Overall, this reflective process has allowed me to critically evaluate my experiences, identify key learning outcomes, and plan for ongoing personal and professional development in machine learning.



---

## References

Chollet, F. (2018) *Deep Learning with Python.* 2nd edn. Shelter Island: Manning Publications.

Goodfellow, I., Bengio, Y. and Courville, A. (2016) *Deep Learning.* Cambridge: MIT Press.

Rolfe, G., Freshwater, D. and Jasper, M. (2001) *Critical Reflection in Nursing and the Helping Professions: A User’s Guide.* Basingstoke: Palgrave Macmillan.

Simonyan, K. and Zisserman, A. (2015) ‘Very Deep Convolutional Networks for Large-Scale Image Recognition.’ *International Conference on Learning Representations (ICLR).* Available at: https://arxiv.org/abs/1409.1556 (Accessed: 13 October 2025).

University of Edinburgh (no date) *Reflection Toolkit.* Available at: https://www.ed.ac.uk/studying/learning-resources/study-skills (Accessed: 13 October 2025).

