# Brain_Age_Prediction_using_Split_Learning

## How to Use

### 1. Open Application File
1) Server program: socket_splitn_server.ipynb file.
2) Client program: socket_splitn_client_{dataset_name}.ipynb file
3) This experiment used CoRR, SALD, and IXI datasets.

### 2. Hyperparameter Setting
The current Epoch is set to 10, User 3, Batch size 5, and num_worker 8.
If you increase the number of users, you can increase the number of learning datasets, but due to GPU problems, not
recommended

### 3. Run the application
First, run the entire Server Side code.
Then, the "Open the Server Socket" of the server program will respond to the clients' responses
Stand by.
At this point, execute the Client Side code one at a time.
When the connection with the client is complete, click "Receive client" to "Connected with (IP address),
Port Number" is output.
When all the clients with the specified number of users are connected, the learning begins.
