# compile for Volta GPU
arch=70

all:
	nvcc -arch=sm_${arch} hello-world.cu -o hello-world

clean:
	rm -rf hello-world

