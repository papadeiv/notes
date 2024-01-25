## Installation
1. Download
```bash
curl -fsSL https://install.julialang.org | sh
```
2. Create symlink
```bash
sudo mkdir -p /usr/local/lib/julia/bin/
sudo ln -s ~/.julia/juliaup/julia-1.10.0+0.x64.linux.gnu/bin/julia /usr/local/lib/julia/bin
```

## Use the package manager
1. Launch the REPL from the terminal
```bash
julia
```
2. Go into Package Manager mode by typing `]`
3. Type the following
```bash
add DynamicalSystems DifferentialEquations Statistics CairoMakie LaTeXStrings ProgressMeter 
```
4. Type `backspace` to go back in Prompt mode and execute `include("filename.jl")`
5. Type `ctrl + d` to exit the REPL
