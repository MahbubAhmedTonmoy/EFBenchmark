``` ini

BenchmarkDotNet=v0.13.2, OS=Windows 10 (10.0.19044.2006/21H2/November2021Update)
Intel Core i5-10400 CPU 2.90GHz, 1 CPU, 12 logical and 6 physical cores
.NET SDK=6.0.400
  [Host]     : .NET 5.0.17 (5.0.1722.21314), X64 RyuJIT AVX2  [AttachedDebugger]
  DefaultJob : .NET 5.0.17 (5.0.1722.21314), X64 RyuJIT AVX2


```
|               Method |         Mean |      Error |     StdDev |       Gen0 |       Gen1 |      Gen2 |    Allocated |
|--------------------- |-------------:|-----------:|-----------:|-----------:|-----------:|----------:|-------------:|
|           GetAuthors | 1,190.874 ms | 17.3747 ms | 16.2523 ms | 30000.0000 | 11000.0000 | 3000.0000 | 182340.68 KB |
| GetAuthors_Optimized |     4.455 ms |  0.0872 ms |  0.0970 ms |     7.8125 |          - |         - |     80.28 KB |
