# Brain_Age_Prediction_using_Split_Learning

## Overview
Due to the perception of data privacy and the increase in individual capacity of data, it is increasingly necessary to achieve learning without sharing data held by clients with servers. And the methodology includes federated learning and split learning, which learn all or part of it inside the client. 

In this repo, based on previous studies on split learning, this learning method was applied to an MRI data brain age prediction algorithm using 3D CNN. In conclusion, the following model was lower than the results of learning in a general way, but it was confirmed that there was a possibility of overcoming it through data augmentation or algorithm improvement.

## How to Use

### 1. Open Application File
1) Server program: socket_splitn_server.ipynb file.
2) Client program: socket_splitn_client_{dataset_name}.ipynb file
3) This experiment used CoRR, SALD, and IXI datasets.

### 2. Hyperparameter Setting
The current Epoch is set to 10, User 3, Batch size 5, and num_worker 8.
If you increase the number of users, you can increase the number of learning datasets

### 3. Run the application
First, run the entire Server Side code.
Then, the "Open the Server Socket" of the server program will respond to the clients' responses
Stand by.
At this point, execute the Client Side code one at a time.
When the connection with the client is complete, click "Receive client" to "Connected with (IP address),
Port Number" is output.
When all the clients with the specified number of users are connected, the learning begins.
