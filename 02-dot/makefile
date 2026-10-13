# compile for Volta GPU
CUDADIR ?= /usr/local/cuda

# gpu architecture
arch=70

LIB=-L${CUDADIR}/lib64 -lcublas

all:
	nvcc -arch=sm_${arch} dot.cu -o dot ${LIB}

clean:
	rm -rf dot

