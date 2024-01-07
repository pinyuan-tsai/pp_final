# Parallel AES Encryption Algorithm
This project contains three versions of AES implementation: serial, OpenMP and CUDA.

## Instruction of Use
### Serial version  
1. compile:  
`g++ serial.cpp -o serial`  
2. run:  
`./serial {input_path} {key_path} {output_path}`  
e.g., `./serial in.txt key.txt serial_out.txt` 

### OpenMP version  
1. compile:  
`g++ omp.cpp -o omp -fopenmp -mavx2`  
2. run:  
`./omp {input_path} {key_path} {output_path}`  
e.g., `./omp in.txt key.txt omp_out.txt`

### CUDA version  
1. compile:  
`nvcc cuda.cu -o cuad`  
2. run:  
`./cuda {input_path} {key_path} {output_path}`  
e.g., `./cuda in.txt key.txt cuda_out.txt` 