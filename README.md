# Derivative free optimization project 

This repository holds the modified ```example_experiment2.py``` file needed to run COCO benchmarking on the DFO-GN algorithm in Python. 
Begin by following the instructions detailed on [https://github.com/numbbo/coco](https://github.com/numbbo/coco).
Make sure to import the dfogn package on the python distribution to be used :
```shell
pip install --pre dfogn
```
Run the file while making sure to modify the variables : ```budget_multiplier```, ```suite_filter_options```, as well as the options for dfogn on line 162 : 
```python
fmin.solve(objfun=problem, x0=propose_x0(), lower=problem.lower_bounds, upper=problem.upper_bounds, maxfun=evalsleft(), rhobeg=itrr)
```  
The folders ```exdata``` and ```ppdata``` contain the data from the executed experiments.  
