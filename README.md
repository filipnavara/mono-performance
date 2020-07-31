# CoreCLR Microbenchmarks

**Due to robbery where the build machine was stolen this project is cancelled for the time being.**

[![Build Status](https://filipnavara.visualstudio.com/mono-performance/_apis/build/status/filipnavara.mono-performance?branchName=master)](https://filipnavara.visualstudio.com/mono-performance/_build/latest?definitionId=4&branchName=master)

This repository holds scripts for daily runs of the [.NET Core microbenchmarks](https://github.com/dotnet/performance)
on CoreCLR and Mono runtimes. The focus is on running the runtimes in .NET 5 platform target and comparing performance
of various configurations. Both [Mono](https://github.com/mono/mono/) and [CoreCLR](https://github.com/dotnet/coreclr)
use latest git revisions from master branch at the start of the benchmark run.

The following configurations are currently tested:
- CoreCLR
- Mono with LLVM JIT
- Mono with mini JIT

They are tested on those machine pools:
- macOS x64 (macOS 10.15, Mac Mini 2018, Core i5-8500B, 32 GB RAM, disabled Turbo Boost)
- Linux arm64 (Ubuntu 18.04, AWS m6g.large instance, AWS Graviton 2, 8 GB RAM)
