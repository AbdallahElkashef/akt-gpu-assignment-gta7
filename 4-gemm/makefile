# gpu architecture
sm=80
GENCODE_SM   = -gencode arch=compute_$(sm),code=sm_$(sm)
GENCODE_COMP = -gencode arch=compute_$(sm),code=compute_$(sm)
CUDADIR ?= /usr/local/cuda

all:
	nvcc $(GENCODE_SM) $(GENCODE_COMP) -L${CUDADIR}/lib64 gemm.cu -o gemm -lcublas

clean:
	rm -rf gemm