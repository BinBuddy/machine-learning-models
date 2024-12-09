# BinBuddy Model Notebooks

This repository is used by the Machine Learning team in the BinBuddy project to develop and test TensorFlow models. Inside this repository, there are notebooks for data preprocessing and model experimentation from each team member.

## Tech Stack

![TensorFlow](https://img.shields.io/badge/TensorFlow-orange?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-red?style=for-the-badge&logo=keras)
![NumPy](https://img.shields.io/badge/NumPy-blue?style=for-the-badge&logo=numpy)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-orange?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pillow](https://img.shields.io/badge/Pillow-purple?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-blue?style=for-the-badge&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-black?style=for-the-badge&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/Seaborn-lightblue?style=for-the-badge&logoColor=white)

## Repository Structure

- **`models/`**: This folder contains notebooks (`.ipynb`) from each ML team member. Each file reflects individual or group experiments on `model development`.
- **`models/[FINAL MODEL]...`** is the final model that are deployed or in consideration of deploying (current deployed model: [MobileNetV3](https://github.com/GitKentC/binbuddy_model_notebooks/blob/main/models/%5BFINAL_MODEL%5Dmobilenetv3large_waste_finetune_64_latest.ipynb))
- **`python-preprocess-data.ipynb`**: This notebook is used to process the initial dataset, including removing `duplicates` and splitting the dataset into `training`, `validation`, and `test` sets (is used in [dataset repository](https://github.com/GitKentC/dataset))
- **`requirements.txt`**: Contains a list of `Python dependencies` required to run the notebooks in this repository.

## How to Run the Repository

Although we recommend running on Google Colab, follow the steps below to run this repository locally:

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
   # For Linux/Mac
   source venv/bin/activate
   
   # For Windows
   venv\Scripts\activate
   ```
   
5. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
6. **Run the notebook to start exploration**
   - **Using `Google Colab` (Recommendation):**
     - Open Google Colab in your browser.
     - Click `File` > `Open notebook`.
     - Select the `GitHub tab` and enter the `URL` of this repository:
       `https://github.com/GitKentC/binbuddy_model_notebooks`
     - Choose the desired notebook file (e.g., `[FINAL_MODEL]mobilenetv3large_waste_finetune_64_latest.ipynb`).
     - Start running the cells in the notebook sequentially, run from **`!! PREDICT FROM HERE !!`** section if you only wanted to test predict function from the model.
     
   - **Using `Jupyter Notebook`:**
     - Open Jupyter Notebook:
       ```bash
       jupyter notebook
       ```
     - Open the desired notebook file (e.g., `[FINAL_MODEL]mobilenetv3large_waste_finetune_64_latest.ipynb`).
     - Click `Kernel` > `Change kernel` and select the appropriate kernel, such as `Python (venv)` that you created earlier.
     - Once the correct kernel is selected, you can start running the cells in the notebook sequentially.
   
   - **Using `VSCode`:**
     - Open VSCode:
       ```bash
       code .
       ```
     - Open the desired notebook file (e.g., `[FINAL_MODEL]mobilenetv3large_waste_finetune_64_latest.ipynb`).
     - At the top of the notebook (in VSCode), click `Kernel` > `Python: Select Interpreter`.
     - Choose the virtual environment you created (`./venv`).
     - Once the correct kernel is selected, you can start running the cells in the notebook sequentially.
   

## Notes

- We recommend using Google Colab to run this notebook for a simpler experience without requiring additional configuration on your device. 
- If you encounter any issues when running the notebooks, ensure that all the packages in `requirements.txt` are installed.
- Make sure the `virtual environment` is active to avoid conflicts with the system's main Python installation.
