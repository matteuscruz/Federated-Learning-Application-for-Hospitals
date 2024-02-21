#### Federated Learning in Embedded Devices for Hospitals
An IoT inteligent application for hospitals that wants to colaborate in Computer Vision models development for medical images processing. 

The research project focuses on developing a Federated Learning (FL) system integrated with Internet of Things (IoT) devices for diagnosing lung diseases, specifically pneumonia, in remote regions with limited access to healthcare facilities. The system utilizes FL to train AI models locally on individual IoT devices, which then send the model weights to a central server for aggregation. This decentralized approach allows for quick and accurate diagnoses while ensuring the privacy and security of patient data.

Key technical details of the project include:

1. Prototype Design: The system is designed to be deployed in remote regions, small towns, and riverside communities. Each IoT device acts as a client in the FL network, with a central server aggregating model updates.
2. Training Process: FL enables the training of AI models on distributed IoT devices, reducing the need for centralized infrastructure. The system uses a simplified model architecture (SqueezeNet) to optimize training on resource-constrained devices.
3. Hardware and Software Components: The project utilizes Raspberry Pi boards for training the FL model and Google Colab for traditional model training. FastAI and Flower frameworks are used for image processing and FL training, respectively.
4. Communication Protocol: gRPC is employed for communication between IoT devices and the central server, facilitating the sharing of model updates through weighted averaging.
5. Challenges and Solutions: The project addresses challenges such as hardware limitations (lack of dedicated GPU on Raspberry Pi), temperature management issues, and training time discrepancies between FL and traditional methods.

The results presented by the training process demonstrate that the FL training process improves the model performance in the same conditions. The accuracy, loss, and error rate in validation set is better than the tradicional method when FL method is implemented in the training process. The Figures below demonstrates graphically how the model performes during the training. 

![Train Loss](https://github.com/matteuscruz/Federated-Learning-Application-for-Hospitals/assets/31227449/c3f8b9af-7073-4447-b14d-362ca618c641)
![Validation Loss (1)](https://github.com/matteuscruz/Federated-Learning-Application-for-Hospitals/assets/31227449/344f4d9e-35a6-4b5d-a51e-850465a47132)
![Accuracy Validation](https://github.com/matteuscruz/Federated-Learning-Application-for-Hospitals/assets/31227449/f7aac6f3-8fd5-488a-8f68-e3915044d72b)
![Error Rate](https://github.com/matteuscruz/Federated-Learning-Application-for-Hospitals/assets/31227449/17b1aa5e-0c9e-431a-a4db-b63c2184bd53)
