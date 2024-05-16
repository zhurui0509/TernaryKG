# TernaryKG
This is for the project of representing and reasoning over ternary projective relations in geospatial knowledge graphs. The relevant paper is published at International Journal of Geographic Information Science [paper](https://www.tandfonline.com/doi/abs/10.1080/13658816.2022.2092115?casa_token=5Rp2xoq8_PcAAAAA:E1WKvoChn4bNmu-5MHGOUfepLVFAqc2F6Cm2Rx_5XsDxjRrx_L6CLaOjpRdOzZRk_OHijx8dZALh_w)

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

## To cite the paper 
@article{zhu2022reasoning,
  title={Reasoning over higher-order qualitative spatial relations via spatially explicit neural networks},
  author={Zhu, Rui and Janowicz, Krzysztof and Cai, Ling and Mai, Gengchen},
  journal={International Journal of Geographical Information Science},
  volume={36},
  number={11},
  pages={2194--2225},
  year={2022},
  publisher={Taylor \& Francis}
}
