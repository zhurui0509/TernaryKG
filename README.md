# TernaryKG
This is for the project of representing and reasoning ternary projective relations in geospatial knowledge graphs.

## Data
We provide three datasets with different densities to experiment the model:


| Name              | # Training  | # Testing | # Validation |
| -----------       | ----------- |-----------|-----------   |
| 2000pairs_10min   | 15895       | 1987     | 1987        |
| 2000pairs_20min   | 31578        | 3947   | 3947        |
| 2000pairs_30min   | 46871       | 5859    | 5859       |


## Script
One can replicate the experiment (Table 4 in the paper) by running the bash script (use the 2000pairs_20min as an example):
```
bash ./code/run_experiment_all.sh
```
The code is built based on https://github.com/eXascaleInfolab/HINGE_code/

## Library reuirement 
* python: 3.6.10
* torch: 1.4.0
* numpy: 1.18.1
* tensorflow-gpu: 2.2.0
* ray: 1.0.1 (optional)

## Platform requirement 
* The experiment was conducted on CUDA with two GPUs, each has a 12GB memory. 
