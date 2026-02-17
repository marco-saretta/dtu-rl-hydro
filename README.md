# Reinforcement Learning for Hydropower Scheduling

DTU Special Course (2.5 ECTS)

This repository contains coursework and experiments on sequential
decision making applied to hydropower systems.

## Overview

Core topics:

-   Markov Decision Processes (MDPs)
-   Policy-based decision making
-   DADS (Discrete Actions, Discrete States)
-   CACS (Continuous Actions, Continuous States)
-   Reinforcement Learning (tabular and neural network methods)
-   Stochastic Dual Dynamic Programming (SDDP)
-   Water value as value function approximation

Final objective: compare RL-based approaches and SDDP for hydropower
scheduling.

## Installation

### Clone

``` bash
git clone https://github.com/marco-saretta/rl-hydropower-scheduling.git
cd rl-hydropower-scheduling
```

### Using uv

``` bash
uv sync
```

### Using Conda

``` bash
conda create -n rl-hydro python=3.11
conda activate rl-hydro
pip install -e .
```

## Course Plan

- Week 1: From Optimization to Policies\
- Week 2: MDP Fundamentals\
- Week 3: DADS and Tabular RL\
- Week 4: CACS and Function Approximation\
- Week 5: Value Functions and Water Value\
- Week 6: SDDP\
- Week 7--8: Hydropower Scheduling Project

## Project structure

The directory structure of the project looks like this:
```txt
├── .github/                  # Github actions and dependabot
│   ├── dependabot.yaml
│   └── workflows/
│       └── tests.yaml
├── configs/                  # Configuration files
├── data/                     # Data directory
│   ├── processed
│   └── raw
├── dockerfiles/              # Dockerfiles
│   ├── api.Dockerfile
│   └── train.Dockerfile
├── docs/                     # Documentation
│   ├── mkdocs.yml
│   └── source/
│       └── index.md
├── models/                   # Trained models
├── notebooks/                # Jupyter notebooks
├── reports/                  # Reports
│   └── figures/
├── src/                      # Source code
│   ├── project_name/
│   │   ├── __init__.py
│   │   ├── api.py
│   │   ├── data.py
│   │   ├── evaluate.py
│   │   ├── models.py
│   │   ├── train.py
│   │   └── visualize.py
└── tests/                    # Tests
│   ├── __init__.py
│   ├── test_api.py
│   ├── test_data.py
│   └── test_model.py
├── .gitignore
├── .pre-commit-config.yaml
├── LICENSE
├── pyproject.toml            # Python project file
├── README.md                 # Project README
└── tasks.py                  # Project tasks
```


## Resources 

- Folder **resources**
- **Textbook:** [Powell – Sequential Decision Analytics and Modeling (2022)](https://castle.princeton.edu/wp-content/uploads/2022/11/Powell-SDAM-Nov242022_final_w_frontcover.pdf)
- **Code:** [Stochastic Optimization GitHub](https://github.com/wbpowell328/stochastic-optimization)
- **DTU course reference:** [RL course](https://02465material.pages.compute.dtu.dk/02465public/index.html)
