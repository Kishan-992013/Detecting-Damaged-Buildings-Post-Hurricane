# Detecting-Damaged-Buildings-Post-Hurricane

After a hurricane, damage assessment is vital for the NGOs, government organizations and rescue operations so that resources and help can be planned and allocated appropriately.
The process of driving down and identifying damaged houses can be labor-intensive and time-consuming and not the most efficient method as well.
Hence in this project, we will be using CNNs through transfer learning to classify buildings using the satellite imagery data.

### Data and Labels
10,000 train images (5,000 damaged and 5,000 non-damaged)
2,000 validation images (1,000 damaged and 1,000 non-damaged)
11,000 test images (9,000 damaged and 2,000 non-damaged)

### Model
Utilised MobileNET architecture with ImageNET weights with used custom fully-connected layers instead of its outer layers. The first ten layers are set to non-trainable to utilise the features it has learned from ImageNET. Training this model for 3 epochs with adam optimizer and categorical_crossentropy loss, achieved 95+% accuracy on test data.

From the results it was concluded that Surroundings play crucial role in classifying the damaged buildings.
