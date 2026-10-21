# compile for Volta GPU
CUDADIR ?= /usr/local/cuda

# gpu architecture
arch=70

LIB=-L${CUDADIR}/lib64 -lcublas

all:
	nvcc -arch=sm_${arch} gemm.cu -o gemm ${LIB}

clean:
	rm -rf gemm

