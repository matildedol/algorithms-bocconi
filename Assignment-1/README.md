The file **recolor.py** implements Lloyd's heuristic algorithm to solve the k-means problem. It outputs a recolored image with k colors.
Usage: python3 recolor.py {input-image} {output-image} {k}

Alternatively, an IP model is designed for the k-means problem and solved exactly with glpk. 
- **IPmodel.pdf** provides a detailed description of the model;
- **datafile_script.py** creates the .dat file of data inputs for the problem;
- **kmeans.mod** specifies the model. 
They should be implemented as:
`python3 datfile_script.py {input-image} {k} {dat-file-path}`
and then to solve the problem with glpk:
`glpsol --model {.mod file} --data {.dat file} --output {optional output file}
