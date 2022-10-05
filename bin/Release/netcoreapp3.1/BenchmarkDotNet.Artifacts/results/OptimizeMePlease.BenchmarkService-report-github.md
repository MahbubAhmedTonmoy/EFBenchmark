``` ini

BenchmarkDotNet=v0.13.2, OS=Windows 10 (10.0.19044.2006/21H2/November2021Update)
Intel Core i5-10400 CPU 2.90GHz, 1 CPU, 12 logical and 6 physical cores
.NET SDK=6.0.400
  [Host]     : .NET Core 3.1.28 (CoreCLR 4.700.22.36202, CoreFX 4.700.22.36301), X64 RyuJIT AVX2  [AttachedDebugger]
  DefaultJob : .NET Core 3.1.28 (CoreCLR 4.700.22.36202, CoreFX 4.700.22.36301), X64 RyuJIT AVX2


```
|               Method |         Mean |      Error |     StdDev |       Median |       Gen0 |       Gen1 |      Gen2 |    Allocated |
|--------------------- |-------------:|-----------:|-----------:|-------------:|-----------:|-----------:|----------:|-------------:|
|           GetAuthors | 1,318.969 ms | 30.0027 ms | 87.0432 ms | 1,282.384 ms | 30000.0000 | 11000.0000 | 3000.0000 | 182801.55 KB |
| GetAuthors_Optimized |     4.437 ms |  0.0197 ms |  0.0154 ms |     4.435 ms |     7.8125 |          - |         - |     90.61 KB |
