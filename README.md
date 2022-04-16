# EMPHCN：Drug repositioning based on the enhanced message passing and hypergraph convolutional networks
## Install
To use EMPHCN you must make sure that your python version is greater than 3.7. If you don’t know the version of python you can check it by:
```python
python
>>> import platform
>>> platform.python_version()
'3.7.13'
```
## Environment Requirement
The required packages are as follows:
- PyTorch==1.7.0
- PyTorch-Geometric==1.5.0
- numpy==1.19.2
- scikit-learn==0.21.3

## Data availability
In the "data" folder, we provide the compressed format of the datasets T1,T2 used in the paper. If you want to use them, please download and unzip them first. 
### T1 datasets
- drug-disease associations in the T1 dataset were selected from ZhangDDA
- sim_pathway.txt: pathway similarity matrix
- sim_target.txt: target similarity matrix
- sim_drug-drug interaction.txt:drug-drug interactions similarity matrix
- sim_enzyme.txt:drug enzymes similarity matrix
- spilt_x.mat:10 cross validation index
- d_p.pt:drug-protein associations
- r_p.pt:diseas-protein associations
- p_p.pt:protein-protein associations
### T2 datasets
- drug-disease associations in the T2 dataset were selected from repoDB
- sim_chemical.txt: chemical similarity matrix
- sim_clinical.txt: clinical similarity matrix
- sim_drugside_effect’s .txt:drugside_effect’s similarity matrix
- spilt_x.mat:10 cross validation index
- d_p.pt:drug-protein associations
- r_p.pt:diseas-protein associations
- p_p.pt:protein-protein associations
## Usage
### Quick start
We use the dataset T1 to illustrate an example. You should first enter the "data" folder and unzip the "T1.zip" file. Then you just need to go back to the EMPHCN file directory and run the following code:

```bash
python main.py --dataset T1
```
##### T2 Datesets

```bash
python main.py --dataset folder_name
```
