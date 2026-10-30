# gpu architecture (Blackwell)
sm=120
GENCODE_SM   = -gencode arch=compute_$(sm),code=sm_$(sm)
GENCODE_COMP = -gencode arch=compute_$(sm),code=compute_$(sm)

all:
	nvcc $(GENCODE_SM) $(GENCODE_COMP) gemm.cu -o gemm.exe -lcublas

clean:
	del gemm.exe