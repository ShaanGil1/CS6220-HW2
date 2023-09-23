# Installation
- Install conda from: https://www.anaconda.com/ <br>
- Install cuda from: https://developer.nvidia.com/cuda-11-7-0-download-archive <br>
- For Nvidia GPU run the following line on command prompt to check cuda version <br>
```
nvcc -V
```
- Extract all files into a folder <br>
- In the root of the folder run the following line using conda command line<br>
```
conda env create -f environment.yml
```
- Sometimes pytorch doesn't install well through .yml files if this happens visit PyTorch website to install that, all other libraries can be installed via "pip install {name of library}"
- Activate the environment using the following command: <br>
```
conda activate HW2
```
- Run the model.ipynb <br>
- Run all cells and the models should run <br>
- Modify any hyperparams in the hyperparams cell, change whatever search space of hyperparams you want to look at<br>
- Note: Dataset only needs to be downloaded once no need to re-run that cell after the first time<br>
- All results will be pasted into a .csv file after model completion
- All needed images will be generated in the cell blocks coresponding to them, save them as needed
# Computer Specs
- GPU: Nvidia RTX 3070 (8GB RAM)
- CPU: AMD Ryzen 5800X 8-Core
- 32 GB DDR4 RAM
# Files
- model.ipynb : File that does everything, download dataset runs models, pastes results into .csv file. Generates Confusion matrices and does Outlier Test Scenario
- HW2_tables.xlsx : Contains all the tables created for the report
- raw_K_probs.txt : Contains Outlier Test Scenario raw probability distributions for all used models
- results.csv : Prints out of all metrics after all models have been run
- environment.yml : env file that has all the used packages/versions
- /report_images : All images used in report
- /k_images : dataset for Outlier Test Scenario
- /models : .pth files for all trained models  (saves all model weights)
- HW2_report.pdf : Contains the full report
