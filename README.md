# hw1p1
Here are the steps to run your code for the project:

---

## Steps to Run the Code

### 1. **Clone or Download the Repository**
   - Ensure you have the `HW1P2_F24_Starter_Notebook.ipynb` file.

### 2. **Install Required Libraries**
   - Before running the notebook, install the necessary dependencies. The primary libraries used are:
     ```bash
     pip install numpy scikit-learn matplotlib torch
     ```

### 3. **Connect your Kaggle API and Download the Data from Kaggle**
   - Commands are already written in .ipynb file.
   - Install and import the chardet

### 4. **Configure Paths and Parameters**
   - Ensure the paths to your dataset (e.g., MFCC features and labels) are correctly set in the notebook. Update the paths in the data loading section if necessary.
   - Run Class AudioDatset
   - Run Class AudioTestDataSet


### 5. **Set the Configuration Parameters**
   - The default configuration is included in the notebook.
     ```python
     
     config = {
         'epochs'        : 20,
         'batch_size'    : 2048,
         'context'       : 35,
         'init_lr'       : 1e-3,
         'weight_decay'  : 1e-3,
         'dropout'       : 0.2
     }
     ```

### 6. **Run the Cells Sequentially**
   - Execute each cell one by one. The notebook is structured to:
     - Load the dataset
     - Define the model architecture, Make sure it is taking 19.43 M parameters
     - Set up the optimizer, loss function, and learning rate scheduler
     - Train the model
     - Evaluate the model's performance on the validation set

### 7. **Monitor Training**
   - While the training process runs, the notebook will output weights and biases. Please check out wandb logs.
- Execute each cell one by one.
   - Creating wandb run
      - username = skandv
      - password =
      - API key = f9cf09dac50889564c1f8fb34fff472412382ff7
   - Saving model arch
   - Displaying Ablations
   - Testing method
   - Predictions
          
### 8. **Evaluate the Model**
   - After training, the notebook includes code to evaluate the model on the test set. Run the evaluation cells to check accuracy, loss, and other metrics.

### 9. **Save or Export Results**
   - The notebook includes cells to save the csv file.
   - Once file is created finish the wandb run

By following these steps, you should be able to run your code and replicate the results generated during development. Let me know if you need further clarification!

Note: I am not able to make my WandDB project public, So I extracted the CSV output from there and screnshot of graphs and created a folder for wandb logs in handin.tar. Please reachout to me for any clarification and I can show the logs live also over zoom or in-person or I can add the grader email ID in my team in wandb to give the access.
