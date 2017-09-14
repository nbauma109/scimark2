build/c/scimark2
**                                                              **
** SciMark2 Numeric Benchmark, see http://math.nist.gov/scimark **
** for details. (Results can be submitted to pozo@nist.gov)     **
**                                                              **
Using       2.00 seconds min time per kenel.
Composite Score:         1305.58
FFT             Mflops:  1108.50    (N=1024)
SOR             Mflops:  1136.37    (100 x 100)
MonteCarlo:     Mflops:   360.80
Sparse matmult  Mflops:  1367.90    (N=1000, nz=5000)
LU              Mflops:  2554.31    (M=100, N=100)
build/c/scimark2 -large
**                                                              **
** SciMark2 Numeric Benchmark, see http://math.nist.gov/scimark **
** for details. (Results can be submitted to pozo@nist.gov)     **
**                                                              **
Using       2.00 seconds min time per kenel.
Composite Score:          966.52
FFT             Mflops:   150.35    (N=1048576)
SOR             Mflops:  1038.17    (1000 x 1000)
MonteCarlo:     Mflops:   383.20
Sparse matmult  Mflops:   844.46    (N=100000, nz=1000000)
LU              Mflops:  2416.42    (M=1000, N=1000)
mkdir -p build/java
javac -sourcepath src/java -d build/java src/java/jnt/scimark2/commandline.java
java -classpath build/java jnt.scimark2.commandline

SciMark 2.0a

Composite Score: 1167.485532434665
FFT (1024): 859.6552993039752
SOR (100x100):   863.71808791014
Monte Carlo : 483.449727694041
Sparse matmult (N=1000, nz=5000): 1090.4493394951912
LU (100x100): 2540.1552077699766

java.vendor: Oracle Corporation
java.version: 1.8.0_131
os.arch: amd64
os.name: Linux
os.version: 4.9.36-x86_64-linode85
java -classpath build/java jnt.scimark2.commandline -large

SciMark 2.0a

Composite Score: 984.1050448836326
FFT (1048576): 136.3783478067598
SOR (1000x1000):   806.1685757367928
Monte Carlo : 515.4785657766312
Sparse matmult (N=100000, nz=1000000): 906.9972883847818
LU (1000x1000): 2555.502446713197

java.vendor: Oracle Corporation
java.version: 1.8.0_131
os.arch: amd64
os.name: Linux
os.version: 4.9.36-x86_64-linode85
