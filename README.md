# Deep learning softare tools benchmark
A benchmark framework for measuring different deep learning tools. Please refer to http://dlbench.comp.hkbu.edu.hk/ for our testing results and more details.

## Introduction
### Overview of **dlbench**    

| Dirctory         	| Description                                      									|
|------------------	|--------------------------------------------------------------------------------	|
| configs/         	| Configuration files for running benchmark                                      	|
| network-configs/ 	| Description of our tested models                                               	|
| synthetic/       	| Our benchmark tests with fake data                                             	|
| tools/           	| Contains running scripts and network configurations of each deep learning tool 	|
| logs/           	| Will be generated by running benchmark.py. Running logs should be put in here 	|

### Run benchmark  
#### Prepare Data  
Prepare data for the tools you want to run and put them under $HOME/data. Note that the name of each data directory should be the same as the name of the tool for convenience.   
You can download data we used for our benchmark on our website.

#### Prepare .config file
There are some sample configuration files in configs/, you can choose one of them as example and change values of each item according to your needs and environment.
#### Run
To run benchmark test just execute   
> **python benchmark.py -config -config configs/\<your config file>.config**

### Add new tools
Follow the instructions in *tools/Readsme.md* preparing the running scripts and netowrk configurations. Note that training data should be put in **$HOME/data/** so that we can test new tools in our machines and update benchmarking results to our website.
