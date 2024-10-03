# hw1p1
Here are the steps to run your code for the project:

---

## Steps to Run the Code

### 1. **Clone or Download the Repository**
   - Ensure you have the `.ipynb` file along with the dataset. If the files are compressed, unzip them first.

### 2. **Install Required Libraries**
   - Before running the notebook, install the necessary dependencies. The primary libraries used are:
     ```bash
     pip install numpy scikit-learn matplotlib torch
     ```

### 3. **Open Jupyter Notebook**
   - Navigate to the directory where your notebook file (`HW1P2_F24_Starter_Notebook.ipynb`) is located. Open the Jupyter notebook in your terminal using:
     ```bash
     jupyter notebook
     ```
   - This will open Jupyter in your web browser. Select the notebook file to open it.

### 4. **Configure Paths and Parameters**
   - Ensure the paths to your dataset (e.g., MFCC features and labels) are correctly set in the notebook. Update the paths in the data loading section if necessary.

### 5. **Set the Configuration Parameters**
   - The default configuration is included in the notebook. You can modify the parameters such as the number of epochs, batch size, learning rate, etc. in the configuration section:
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
     - Define the model architecture
     - Set up the optimizer, loss function, and learning rate scheduler
     - Train the model
     - Evaluate the model's performance on the validation set

### 7. **Monitor Training**
   - While the training process runs, the notebook will output the loss and accuracy for each epoch. Ensure your GPU is being utilized if available. If training takes too long, consider enabling **mixed precision training** for better efficiency.

### 8. **Evaluate the Model**
   - After training, the notebook includes code to evaluate the model on the test set. Run the evaluation cells to check accuracy, loss, and other metrics.

### 9. **Save or Export Results**
   - The notebook includes cells to visualize and save model performance (e.g., accuracy plots, loss curves). Save any figures or trained model checkpoints as needed.

---

By following these steps, you should be able to run your code and replicate the results generated during development. Let me know if you need further clarification!
