# Cloverleaf-in-Azure

# Create a HPC VM in Azure (e.g. H16r) 

Use CentOS 7.4 HPC as image


# Cre

get the source code from

git clone https://github.com/UK-MAC/Cloverleaf3D_ref.git 


```
cd Cloverleaf
export I_MPI_CXX=g++
export I_MPI_CC=gcc
export I_MPI_FC=gfortran
export I_MPI_F90=gfortran

make COMPILER=GNU


``` 
