EXECS=mpi_hello_world
MPICC?=mpicc

all: ${EXECS}

mpi_hello_world: mpi_hello_world.c
	${MPICC} -static -L../../../../pisces/hobbes/libhobbes -o mpi_hello_world mpi_hello_world.c -lmpi -lopen-rte -lopen-pal -lhobbes -lrt -lutil -lm

clean:
	rm -f ${EXECS}
