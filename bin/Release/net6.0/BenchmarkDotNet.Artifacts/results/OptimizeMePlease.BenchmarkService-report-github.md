``` ini

BenchmarkDotNet=v0.13.2, OS=Windows 10 (10.0.19044.2006/21H2/November2021Update)
Intel Core i5-10400 CPU 2.90GHz, 1 CPU, 12 logical and 6 physical cores
.NET SDK=6.0.400
  [Host]     : .NET 6.0.8 (6.0.822.36306), X64 RyuJIT AVX2  [AttachedDebugger]
  DefaultJob : .NET 6.0.8 (6.0.822.36306), X64 RyuJIT AVX2


```
|               Method |         Mean |      Error |     StdDev |       Gen0 |       Gen1 |      Gen2 |    Allocated |
|--------------------- |-------------:|-----------:|-----------:|-----------:|-----------:|----------:|-------------:|
|           GetAuthors | 1,220.601 ms | 24.3634 ms | 71.0693 ms | 31000.0000 | 11000.0000 | 3000.0000 | 188489.11 KB |
| GetAuthors_Optimized |     3.948 ms |  0.0490 ms |  0.0409 ms |    15.6250 |          - |         - |    121.07 KB |
