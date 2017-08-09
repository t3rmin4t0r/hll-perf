# HyperLogLog benchmark


```
mvn clean package
java -jar target/benchmarks.jar -prof gc

Benchmark                             Mode  Cnt   Score    Error  Units
HllBenchmark.benchBuild               avgt   10  ≈ 10⁻³           ms/op
HllBenchmark.benchDeserialize         avgt   10   1.505 ±  0.093  ms/op
HllBenchmark.benchDeserializeNonSync  avgt   10   1.383 ±  0.051  ms/op
HllBenchmark.benchMergeDenseToDense   avgt   10   0.008 ±  0.001  ms/op
HllBenchmark.benchMergeDenseToEmpty   avgt   10   1.272 ±  0.040  ms/op
HllBenchmark.benchMergeDenseToSparse  avgt   10   0.008 ±  0.001  ms/op
HllBenchmark.benchMergeEmptyToDense   avgt   10   0.025 ±  0.001  ms/op
HllBenchmark.benchMergeEmptyToSparse  avgt   10  ≈ 10⁻³           ms/op
HllBenchmark.benchMergeSparseToDense  avgt   10   0.030 ±  0.001  ms/op
HllBenchmark.benchMergeSparseToEmpty  avgt   10   0.001 ±  0.001  ms/op
```
