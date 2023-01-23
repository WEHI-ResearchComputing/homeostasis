# An agent based model of cell population homeostasis

Population homeostasis in the presence of a division and signals driving Myc production.

## To setup
```
julia> ]
pkg> dev  https://github.com/cyton-dynamics/cyton.toolkit.git
```
Exit Julia and in bash change git branch

```
$ cd ~/.julia/dev/Cyton/
$ git checkout globalagents

```
Then back to the project folder
```
julia> ]
pkg> add Cairo, Fontconfig,DataFrames, Gadfly, Statistics, Serialization, ArgParse

```
## To test run, in Julia REPL
```
julia> using Cyton

julia> include("run.jl")
main (generic function with 1 method)

julia> parms = TrialParameters(1,0.1,10)
trial=1 startPopulation=10 threshold=0.1

julia> doRun(parms)
```