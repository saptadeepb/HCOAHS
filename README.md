# 🦞 HCOAHS: Hybrid Crayfish Optimization Algorithm with Harmony Search

## 📘 Overview

**HCOAHS** is a novel **hybrid metaheuristic optimization algorithm** that integrates the **Crayfish Optimization Algorithm (COA)** with **Harmony Search (HS)** to achieve robust global–local balance and improved optimization accuracy.  
The algorithm introduces temperature-adaptive phase control, harmony memory seeding, and coordinated parameter adaptation to prevent premature convergence and enhance solution quality.

> ⚠️ **Note:** This repository contains research code supporting a manuscript currently under peer review. Please contact the authors before citing or distributing.

---

## ✨ Key Features

- 🔄 **Temperature-adaptive phase control** – smooth switching between exploration and exploitation  
- 🧠 **Population-seeded harmony memory** – initialized using top-performing COA agents  
- 🎵 **Phase-specific HS refinement** – active only during exploitation phases  
- ⚙️ **Coordinated parameter adaptation** – coupled control of COA and HS parameters for stable convergence  

---

## 🚀 Quick Start (MATLAB Example)

```matlab
% Define objective function
objFunction = @(x) sum(x.^2);

% Define problem parameters
dim = 30;                         % Problem dimension
lb = -100 * ones(1, dim);         % Lower bounds
ub = 100 * ones(1, dim);          % Upper bounds

% Algorithm settings
N = 30;                           % Population size
T = 500;                          % Maximum iterations

% Run HCOAHS
[bestFitness, bestSolution, convergence] = HCOAHS(objFunction, N, T, dim, lb, ub);

fprintf('Best Fitness: %.6e\n', bestFitness);
📬 Contact
For code-related queries, please contact:
Binanda Maiti – mathematicsbinanda@gmail.com 
Dr. Saptadeep Biswas – saptadeepbiswas7@gmail.com
