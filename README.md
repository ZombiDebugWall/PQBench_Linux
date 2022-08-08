# PQBench_Linux

Simple benchmark which benches your single core CPU performance using the pq-formula.

## Compilation and installation
I am not responsible for any hardware damage, you run this programm on your own risk!

PQBench can be compiled using the g++ compiler on linux:

```
$ g++ mainpqthread.cpp -o pqbench
```

And installed by moving the executable into the bin folder:

```
$ sudo mv pqbench /bin/pqbench
```

Or alternatively just run directly in the compilation folder:
```
$ ./pqbench
```
## Arguments

PQBench provides following arguments:
```
-t, 	--time

-cs, 	--check-status

-oc,	--overclocking

-h	--help
```

### Explaination

```
-t, 	--time (Default active parameter, when run without any arguments)
```
Measures the time that has been taken to to make 1\*10^9 calculations.
The results are displayed in milliseconds, seconds and calculations per millisecond. 
```
-cs, 	--check-status
```
The --check-status parameter can be used to verfiy the benchmark is running and not freezing.
**NOTE:** Due to extra threads running in the background, I recommand to use -t for proper benching.
```
-oc,	--overclocking
```
This parameter can be used for realtime overclocking. It displays calculations per second in realtime and these will change during changing any CPU properties (e.g. CPU frequency). **NOTE:** Due to extra threads running in the background, I recommand to use -t for resonable results (after playing around with your CPU settings).
```
-h	--help
```
It's the --help parameter, what do you expect.
