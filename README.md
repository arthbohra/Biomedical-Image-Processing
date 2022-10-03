# Biomedical-Image-Processing

In this project, I analyzed the MRI scans of brains. Utilizing computer vision, deep learning, and transfer learning, we predicted whether there was a tumor present with over 95 percent accuracy.

**Packages Used**

- Tensorflow/Keras
- OpenCV
- Numpy
- MatPlotLib
- SkLearn

**Results**

<img width="516" alt="Screen Shot 2022-10-02 at 8 17 00 PM" src="https://user-images.githubusercontent.com/47287313/193498021-36ed47eb-e282-449c-bd42-9786ab8f4495.png">


![Unknown](https://user-images.githubusercontent.com/47287313/193498167-5cdffb1e-7175-4408-9509-34c0630b04fe.png)


**Neural Network**

In this neural network, I used pre-trained weights from the image-net model. I added several other layers to the Sequential Model in order to produce this final design:

<img width="400" alt="Screen Shot 2022-10-02 at 8 16 56 PM" src="https://user-images.githubusercontent.com/47287313/193498054-3e22b7a4-077a-4405-9065-99a250f41a12.png">

**The Process**

1. Loading a [Dataset](https://www.kaggle.com/datasets/abhranta/brain-tumor-detection-mri) in from Kaggle: 

2. Observing how the Data Could be Visualized: Using matplotlib and opencv

![Unknown-3](https://user-images.githubusercontent.com/47287313/193497849-5017ea1f-99b9-4918-9bc9-24f53ef0e733.png)

3. Splitting the Dataset into training, validation, and testing folders.

4. Observe the Distribtution of the Dataset (between training, validation, and testing)

![Unknown-2](https://user-images.githubusercontent.com/47287313/193497869-f7421498-62df-4367-b605-43bf8d993cd7.png)

5. Crop the Images using Edge Detection (OpenCV) 

![Unknown-5](https://user-images.githubusercontent.com/47287313/193498558-2c5929cd-7a85-443d-8c10-5dce66f3fcd3.png)

6. Augment the Data: Due to the limited number of MRI scans, we augment the dataset (transforming it, flipping it, rotating it) to increase our sample sizes.

![Unknown-6](https://user-images.githubusercontent.com/47287313/193498821-a724f081-df15-49d0-80fb-af357531052e.png)

7. Design Our Neural Network, Input Training, Validation Sets to Train the Neural Network. 

