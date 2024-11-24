# BinBuddy Model Notebooks

This repository is used by the Machine Learning team in the BinBuddy project to develop and test TensorFlow models. Inside this repository, there are notebooks for data preprocessing and model experimentation from each team member.

## Repository Structure

- **`models/`**: This folder contains notebooks (`.ipynb`) from each ML team member. Each file reflects individual or group experiments on `model development`.
- **`python-preprocess-data.ipynb`**: This notebook is used to process the initial dataset, including removing `duplicates` and splitting the dataset into `training`, `validation`, and `test` sets.
- **`requirements.txt`**: Contains a list of `Python dependencies` required to run the notebooks in this repository.

## How to Run the Repository

Follow the steps below to run this repository locally:

1. **Clone this repository to your local machine**
   ```bash
   git clone https://github.com/GitKentC/binbuddy_model_notebooks.git
   ```
   
2. **Navigate to the repository directory**
   ```bash
   cd binbuddy_model_notebooks
   ```
   
3. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```
   
4. **Activate the virtual environment**
   ```bash
   # Untuk Linux/Mac
   source venv/bin/activate
   
   # Untuk Windows
   venv\Scripts\activate
   ```
   
5. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
6. **Run the notebook to start exploration**
   - **If using `Jupyter Notebook`:**
     - Open Jupyter Notebook:
       ```bash
       jupyter notebook
       ```
     - Open the desired notebook file (e.g., `efficientnetv2_b2_waste_finetune_64.ipynb`).
     - Click `Kernel` > `Change kernel` and select the appropriate kernel, such as `Python (venv)` that you created earlier.
     - Once the correct kernel is selected, you can start running the cells in the notebook sequentially.
   
   - **If using `VSCode`:**
     - Open VSCode:
       ```bash
       code .
       ```
     - Open the desired notebook file (e.g., `efficientnetv2_b2_waste_finetune_64.ipynb`).
     - At the top of the notebook (in VSCode), click `Kernel` > `Python: Select Interpreter`.
     - Choose the virtual environment you created (`./venv`).
     - Once the correct kernel is selected, you can start running the cells in the notebook sequentially.
   
   - **If using `Google Colab`:**
     - Open Google Colab in your browser.
     - Click `File` > `Open notebook`.
     - Select the `GitHub tab` and enter the `URL` of this repository:
       `https://github.com/GitKentC/binbuddy_model_notebooks`
     - Choose the desired notebook file (e.g., `efficientnetv2_b2_waste_finetune_64.ipynb`).
     - Start running the cells in the notebook sequentially.

## Notes

- If you encounter any issues when running the notebooks, ensure that all the packages in `requirements.txt` are installed.
- Make sure the `virtual environment` is active to avoid conflicts with the system's main Python installation.
