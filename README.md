# kongara_Task_1

# Step 1: Data Loading
The implementation starts by reading the CSV files "data.csv" and "label.csv" using the Pandas library. The data and labels are loaded into appropriate data structures to be used for further processing.

# Step 2: Data Preprocessing
From the "data.csv" file, specific columns "ACC X" and "Light" are selected. These columns are chosen based on their relevance to the task. Further preprocessing such as normalization or data augmentation could be added here if needed.

# Step 3: Convolution Neural Network (CNN)
A CNN is defined in this step. The CNN architecture includes:

A convolutional layer with a kernel size of 3 and 8 filters. This layer extracts features from the input data.
A max-pooling layer with a pool size of 2. This layer reduces the spatial dimensions of the features.
A flatten layer that converts the 2D feature maps into a 1D array.
A dense layer that utilizes the softmax activation function for classification.
Step 4: Model Compilation
The defined CNN model is compiled in this step. The compilation includes specifying the loss function, optimizer, and evaluation metrics. In this implementation, the RMSprop optimizer is used.

# Step 5: Model Training
The training process involves feeding the preprocessed data into the CNN model. The model is trained over multiple epochs to iteratively learn the patterns and features present in the data. The training process continues until the model converges. In this case, convergence is observed around the 9th epoch due to the relatively small dataset size.

# Step 6: Batch Size
A batch size of 1 is considered in this implementation, meaning that each data point is processed individually. This choice is made based on the assumption that the dataset is small enough to fit into memory and the intention is to allow the model to learn from each individual instance effectively.

# Step 7: Model Saving
Once the model is trained and converged, it is saved to the "output.txt" file. This saved model can be used later for making predictions on new, unseen data.


