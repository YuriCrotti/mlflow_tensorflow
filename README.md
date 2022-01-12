## Managing ML-lifecycle with MLflow

### Installation 

0. Clone this repository using git or download using Github interface

1. Install conda distribution for python 

2. Open Anaconda Prompt navigate and install requirements: 
    
    - **Optional**: you can create separate conda environment for this tutorial from environment file: 
        ```
        conda env create -f environment.yaml
        ```
        ```
        conda activate mlflowtf
        ```
    - Installing requirements from requirements.txt file:
        ```
        pip install -r requirements.txt
        ```
3. Launch Jupyter notebook from:
    ```
    jupyter notebook
    ```
    
4. Launch MLflow server:
    ```
    mlflow server --backend-store-uri="sqlite:///C:\\path\\to\\project_folder\\backend\\mlflow_data.db" 
                  --default-artifact-root="file:///C:\\path\\to\\project_folder\\artifact_store\\"
    ```
    - Parameters:
        - backend-store-uri - URI to which to persist experiment and run data (sqlite database in our case).
        - default-artifact-root - Local or S3 URI to store artifacts, for new experiments (local folder in our case). 
    
    
5. Make sure that you can access mlflow server and jupyter notebook from your browser :
    - mlflow server   : http://localhost:5000/
    - jupyter notebook: http://localhost:8888/ 

