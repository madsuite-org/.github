<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="madsuite-logo-dark.svg">
    <img src="madsuite-logo.svg" alt="MadSuite" width="360">
  </picture>
</p>

MadSuite is a suite of open-source optimization software for GPUs, written in [Julia](https://julialang.org). It covers algebraic modeling, nonlinear and linear programming solvers, and domain-specific modeling libraries. Website: [madsuite.org](https://madsuite.org).

### Solvers

| Package | Description |
|---|---|
| [MadNLP.jl](https://github.com/madsuite-org/MadNLP.jl) | Nonlinear programming solver (filter line-search interior-point method) with GPU support |
| [MadIPM.jl](https://github.com/madsuite-org/MadIPM.jl) | Linear and quadratic programming solver (Mehrotra predictor-corrector) with GPU support |
| [MadNCL.jl](https://github.com/madsuite-org/MadNCL.jl) | Algorithm NCL as a MadNLP.jl extension, for infeasible or degenerate problems |
| [CCOpt.jl](https://github.com/madsuite-org/CCOpt.jl) | Solver for mathematical programs with complementarity constraints (MPCCs) |

### Modeling abstractions and algebraic modeling systems

| Package | Description |
|---|---|
| [ExaModels.jl](https://github.com/madsuite-org/ExaModels.jl) | Algebraic modeling and automatic differentiation for GPUs, based on a SIMD abstraction of nonlinear programs |
| [ParametricNLPModels.jl](https://github.com/madsuite-org/ParametricNLPModels.jl) | Parametric sensitivities for NLPModels.jl models |
| [MPCCModels.jl](https://github.com/madsuite-org/MPCCModels.jl) | NLPModels.jl extension for modeling MPCCs, used by CCOpt.jl |
| [NLPModelsExtensions.jl](https://github.com/madsuite-org/NLPModelsExtensions.jl) | Extensions to NLPModels.jl |
| [ExaPowerIO.jl](https://github.com/madsuite-org/ExaPowerIO.jl) | Minimal reader for the MATPOWER power system data format |

### Domain-specific libraries

| Package | Description |
|---|---|
| [ExaModelsPower.jl](https://github.com/madsuite-org/ExaModelsPower.jl) | Optimal power flow models built on ExaModels.jl |
| [ExaModelsCollocation.jl](https://github.com/madsuite-org/ExaModelsCollocation.jl) | Transcription of differential equations into algebraic constraints in ExaModels.jl |

### Other tools

| Package | Description |
|---|---|
| [madsuite-py](https://github.com/madsuite-org/madsuite-py) | Python interface to ExaModels.jl |
| [MadCheck.jl](https://github.com/madsuite-org/MadCheck.jl) | Automatic diagnosis tool for nonlinear programs |

### Benchmark libraries

| Package | Description |
|---|---|
| [COPSBenchmark.jl](https://github.com/madsuite-org/COPSBenchmark.jl) | The COPS benchmark for nonlinear optimization, with JuMP and ExaModels backends |
| [ExaCUTEst.jl](https://github.com/madsuite-org/ExaCUTEst.jl) | The CUTEst test set as ExaModels, on the CPU or a GPU |
| [ExaModelsSIF.jl](https://github.com/madsuite-org/ExaModelsSIF.jl) | Pure-Julia SIF decoder: CUTEst problems as native ExaModels |
| [ExaMittelmann.jl](https://github.com/madsuite-org/ExaMittelmann.jl) | Mittelmann's AMPL-NLP benchmark instances as ExaModels |
| [LuksanVlcekBenchmark.jl](https://github.com/madsuite-org/LuksanVlcekBenchmark.jl) | Lukšan-Vlček scalable test problems as ExaModels |
| [MPCCbenchmark.jl](https://github.com/madsuite-org/MPCCbenchmark.jl) | Large-scale mathematical programs with complementarity constraints |
| [MadNLPBenchmark.jl](https://github.com/madsuite-org/MadNLPBenchmark.jl) | Baseline benchmark for tracking MadNLP.jl performance across commits |

Each package's README lists how to cite it.
