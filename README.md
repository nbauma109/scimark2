build/c/scimark2
**                                                              **
** SciMark2 Numeric Benchmark, see http://math.nist.gov/scimark **
** for details. (Results can be submitted to pozo@nist.gov)     **
**                                                              **
Using       2.00 seconds min time per kenel.
Composite Score:         1511.02
FFT             Mflops:  1355.28    (N=1024)
SOR             Mflops:  1497.25    (100 x 100)
MonteCarlo:     Mflops:   334.08
Sparse matmult  Mflops:  1954.11    (N=1000, nz=5000)
LU              Mflops:  2414.38    (M=100, N=100)
build/c/scimark2 -large
**                                                              **
** SciMark2 Numeric Benchmark, see http://math.nist.gov/scimark **
** for details. (Results can be submitted to pozo@nist.gov)     **
**                                                              **
Using       2.00 seconds min time per kenel.
Composite Score:         1115.57
FFT             Mflops:   185.28    (N=1048576)
SOR             Mflops:  1328.36    (1000 x 1000)
MonteCarlo:     Mflops:   334.08
Sparse matmult  Mflops:  1450.94    (N=100000, nz=1000000)
LU              Mflops:  2279.20    (M=1000, N=1000)
javac -sourcepath src/java -d build/java src/java/jnt/scimark2/commandline.java
java -classpath build/java jnt.scimark2.commandline

SciMark 2.0a

Composite Score: 1828.147392244037
FFT (1024): 1049.1672872095655
SOR (100x100):   1239.9968667860549
Monte Carlo : 725.5012230825422
Sparse matmult (N=1000, nz=5000): 1742.9787830855328
LU (100x100): 4383.09280105649

java.vendor: Oracle Corporation
java.version: 1.8.0_131
os.arch: amd64
os.name: Windows 7
os.version: 6.1
java -classpath build/java jnt.scimark2.commandline -large

SciMark 2.0a

Composite Score: 1171.893612057482
FFT (1048576): 201.61114996699823
SOR (1000x1000):   1110.4161167432255
Monte Carlo : 729.4441724952741
Sparse matmult (N=100000, nz=1000000): 1314.0841122732031
LU (1000x1000): 2503.9125088087085

java.vendor: Oracle Corporation
java.version: 1.8.0_131
os.arch: amd64
os.name: Windows 7
os.version: 6.1
