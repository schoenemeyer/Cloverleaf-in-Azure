# Cloverleaf-in-Azure

# Create a HPC VM in Azure (e.g. H16r) 

Use CentOS 7.4 HPC as image


# Cre

get the source code from

git clone https://github.com/UK-MAC/Cloverleaf3D_ref.git 


sudo yum -y install centos-release-scl
sudo yum -y install devtoolset-4-gcc*
scl enable devtoolset-4 bash 

```
cd Cloverleaf
export I_MPI_CXX=g++
export I_MPI_CC=gcc
export I_MPI_FC=gfortran
export I_MPI_F90=gfortran

make COMPILER=GNU

``` 

Testdata can be downloaded from 
https://github.com/Mantevo/CloverLeaf/tree/master/mpi/InputDecks

cp clover_bm16_short.in clover.in 
OMP_NUM_THREADS=1 mpirun -np 16 ./clover_leaf

