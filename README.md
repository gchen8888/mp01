# Mini-Project 1: Dissolved Oxygen with Multiple Effluents

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This is the repository for Mini-Project 1 for [BEE 4750](https://envsys.viveks.me/), taught at [Cornell University](https://cornell.edu) in Fall 2026 by [Vivek Srikrishnan](https://viveks.me).

If enrolled in the class, a PDF of your report should be submitted to Gradescope *no later* than the due date at 9:00pm. Submitting up to 24 hours late will result in a 50% penalty. Students in BEE 4750 may work in groups of 2; students in BEE 5750 work individually.

## Learning Objectives

After completing this mini-project, students will be able to:

- simulate dissolved oxygen concentrations across several effluents;
- recognize when the closed-form Streeter-Phelps solution stops applying and when discretization is necessary;
- determine whether a treatment plan complies with a standard, and explain where the critical value falls and why;
- propagate an uncertain load through the model by Monte Carlo;
- compare sampling error against discretization error in the same model;
- recommend a plan and defend it on grounds the model alone does not supply.

## Repository Overview

The repository consists of the following files:

- `mp01.ipynb`: Jupyter Notebook for the mini-project, including the system data. This is the only file you should need to edit.
- `mp01.pdf`: PDF version of the mini-project for students who don'tm want to rely on the Jupyter Notebook.
- `Project.toml`, `Manifest.toml`: Julia environment files. These should just work, but feel free to add other packages as needed using the `Pkg` package manager. This is the only other file that you might typically end up making changes to, though you should do this using `Pkg`, not directly.
- `mp01.qmd`: Source file for Jupyter notebook generation. You shouldn't need to or want to touch this unless you use Quarto to write your report; everything is in the `.ipynb` file.
- `LICENSE`: This material is licensed using the MIT license. You can ignore this for working on the project.
- `README.md`: This file. You shouldn't need to touch this.
- `.gitignore`: This tells `git` what files to ignore. You shouldn't need to touch this.

## Dependencies

This notebook was written using Julia 1.11.5, and depends on the following packages:
- `Distributions.jl`
- `Plots.jl`
- `LaTeXStrings.jl`
- `IJulia.jl` (runs the notebook; no cell loads it, but keep it in the environment)

## Prerequisites

1. [Install Julia](https://julialang.org/downloads/) before beginning this assignment. This notebook was developed with version 1.11.5, but any 1.11.x should work (there could be some issues with other versions, depending on what's changed; if that occurs, delete `Manifest.toml` before re-evaluating the first notebook cell).
2. If necessary, [install git](https://happygitwithr.com/install-git.html) and [create a GitHub account](https://github.com).
