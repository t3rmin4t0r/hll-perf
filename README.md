# HyperLogLog benchmark


```
mvn clean package
java -jar target/benchmarks.jar -prof gc


Benchmark                                                              Mode  Cnt       Score       Error   Units
HllBenchmark.benchBuild                                                avgt   10      ≈ 10⁻³               ms/op
HllBenchmark.benchBuild:·gc.alloc.rate                                 avgt   10    9845.236 ±   237.788  MB/sec
HllBenchmark.benchBuild:·gc.alloc.rate.norm                            avgt   10    4264.000 ±     0.001    B/op
HllBenchmark.benchBuild:·gc.churn.PS_Eden_Space                        avgt   10    9836.325 ±   383.263  MB/sec
HllBenchmark.benchBuild:·gc.churn.PS_Eden_Space.norm                   avgt   10    4260.345 ±   145.618    B/op
HllBenchmark.benchBuild:·gc.churn.PS_Survivor_Space                    avgt   10       0.340 ±     0.108  MB/sec
HllBenchmark.benchBuild:·gc.churn.PS_Survivor_Space.norm               avgt   10       0.147 ±     0.045    B/op
HllBenchmark.benchBuild:·gc.count                                      avgt   10     217.000              counts
HllBenchmark.benchBuild:·gc.time                                       avgt   10      95.000                  ms
HllBenchmark.benchDeserialize                                          avgt   10       1.476 ±     0.076   ms/op
HllBenchmark.benchDeserialize:·gc.alloc.rate                           avgt   10     155.921 ±     7.833  MB/sec
HllBenchmark.benchDeserialize:·gc.alloc.rate.norm                      avgt   10  241083.025 ±     6.203    B/op
HllBenchmark.benchDeserialize:·gc.churn.PS_Eden_Space                  avgt   10     156.948 ±     8.244  MB/sec
HllBenchmark.benchDeserialize:·gc.churn.PS_Eden_Space.norm             avgt   10  242774.251 ± 11778.279    B/op
HllBenchmark.benchDeserialize:·gc.churn.PS_Survivor_Space              avgt   10       0.627 ±     0.184  MB/sec
HllBenchmark.benchDeserialize:·gc.churn.PS_Survivor_Space.norm         avgt   10     972.569 ±   302.950    B/op
HllBenchmark.benchDeserialize:·gc.count                                avgt   10     156.000              counts
HllBenchmark.benchDeserialize:·gc.time                                 avgt   10      71.000                  ms
HllBenchmark.benchDeserializeNonSync                                   avgt   10       1.381 ±     0.039   ms/op
HllBenchmark.benchDeserializeNonSync:·gc.alloc.rate                    avgt   10     113.293 ±     3.160  MB/sec
HllBenchmark.benchDeserializeNonSync:·gc.alloc.rate.norm               avgt   10  164066.848 ±     5.995    B/op
HllBenchmark.benchDeserializeNonSync:·gc.churn.PS_Eden_Space           avgt   10     114.373 ±     8.596  MB/sec
HllBenchmark.benchDeserializeNonSync:·gc.churn.PS_Eden_Space.norm      avgt   10  165600.589 ± 10306.977    B/op
HllBenchmark.benchDeserializeNonSync:·gc.churn.PS_Survivor_Space       avgt   10       0.565 ±     0.094  MB/sec
HllBenchmark.benchDeserializeNonSync:·gc.churn.PS_Survivor_Space.norm  avgt   10     818.067 ±   133.817    B/op
HllBenchmark.benchDeserializeNonSync:·gc.count                         avgt   10     112.000              counts
HllBenchmark.benchDeserializeNonSync:·gc.time                          avgt   10      53.000                  ms
HllBenchmark.benchMergeDenseToDense                                    avgt   10       0.008 ±     0.001   ms/op
HllBenchmark.benchMergeDenseToDense:·gc.alloc.rate                     avgt   10       0.001 ±     0.001  MB/sec
HllBenchmark.benchMergeDenseToDense:·gc.alloc.rate.norm                avgt   10       0.009 ±     0.001    B/op
HllBenchmark.benchMergeDenseToDense:·gc.count                          avgt   10         ≈ 0              counts
HllBenchmark.benchMergeDenseToSparse                                   avgt   10       0.008 ±     0.001   ms/op
HllBenchmark.benchMergeDenseToSparse:·gc.alloc.rate                    avgt   10       0.001 ±     0.001  MB/sec
HllBenchmark.benchMergeDenseToSparse:·gc.alloc.rate.norm               avgt   10       0.009 ±     0.001    B/op
HllBenchmark.benchMergeDenseToSparse:·gc.count                         avgt   10         ≈ 0              counts
HllBenchmark.benchMergeSparseToDense                                   avgt   10       0.030 ±     0.001   ms/op
HllBenchmark.benchMergeSparseToDense:·gc.alloc.rate                    avgt   10    4700.169 ±   118.496  MB/sec
HllBenchmark.benchMergeSparseToDense:·gc.alloc.rate.norm               avgt   10  147528.035 ±     0.002    B/op
HllBenchmark.benchMergeSparseToDense:·gc.churn.PS_Eden_Space           avgt   10    4696.218 ±   188.763  MB/sec
HllBenchmark.benchMergeSparseToDense:·gc.churn.PS_Eden_Space.norm      avgt   10  147410.683 ±  5134.217    B/op
HllBenchmark.benchMergeSparseToDense:·gc.churn.PS_Survivor_Space       avgt   10       0.288 ±     0.103  MB/sec
HllBenchmark.benchMergeSparseToDense:·gc.churn.PS_Survivor_Space.norm  avgt   10       9.042 ±     3.183    B/op
HllBenchmark.benchMergeSparseToDense:·gc.count                         avgt   10     223.000              counts
HllBenchmark.benchMergeSparseToDense:·gc.time                          avgt   10      96.000                  ms
```
