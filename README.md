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
- Sometimes pytorch does install well through .yaml files if this happens visit PyTorch website to install that, all other libraries can be installed via "pip install {name of library}"
- Activate the environment using the following command: <br>
```
conda activate HW2
```
- Run the model.ipynb <br>
- Run all cells and the model should run <br>
- Modify any hyperparams in the hyperparams cell<br>
- Note: Dataset only needs to be downloaded once no need to re-run that cell after the first time<br>
- All results will be pasted into a .csv file after model completion
- All needed images will be generated in the cell blocks coresponding to them
# Computer Specs
- GPU: Nvidia RTX 3070 (8GB RAM)
- CPU: AMD Ryzen 5800X 8-Core
- 32 GB DDR4 RAM
# Files
- model.ipynb : File that does everything, creates dataset runs models, and finally pastes results into .csv file (also generates pictures + does Outlier Test Scenario)
