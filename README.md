# IIM Project – Reshuffling

## Full Paper: Check this to obtain full information 
[Full Paper](https://drive.google.com/file/d/1lgLWGVcxmSeS5DLZya3z_G53ABxX-nCb/view?usp=drive_link)

## Intro
A collection of notebooks and utilities for exploring warehouse/robot path planning and item reshuffling strategies 
- Integer Programming Models (Kiva, Puzzle-based system (obstacle view), Puzzle-based system (space view))
- Across multiple algorithms (BFS, Greedy, GA, PSO, DQN, MAAC variants), 
- Dataset generators and preprocessing utilities.

## Repository Structure
- **Notebooks**
  - `algo_bfs.ipynb` – Breadth-first search baseline.
  - `algo_greedy.ipynb` – Greedy heuristic approach.
  - `algo_ga.ipynb` / `algo_ga_4x4.ipynb` – Genetic Algorithm experiments (incl. 4x4 setup).
  - `algo_pso.ipynb` – Particle Swarm Optimization approach.
  - `model_kiva.ipynb`, `model_spa.ipynb`, `model_obs.ipynb` – Integer Programming Model for kiva system, puzzle-based system (obstacle view), puzzle-based system (space view).
  - `preprocess_*.ipynb`, `input_generator*.ipynb`, `output_*.ipynb` – Data preparation, input generation, and results processing.
- **Data**
  - `3x3.csv`, `4x4.csv`, `5x5.csv` – Experiment Outcome.
  - `data_graphform.zip` – Graph-form dataset (compressed).
- **Code**
  - `utils/` – Helper modules / Lab.
  - `heuristic/` – Heuristic-related helpers / Lab.
  - `tar4/` – Additional resources and scripts / Lab.
- **Figures**
  - `time_space_network.png`, `障礙物觀點.png` – Visualization.

## Quick Start
- Use Python 3.9+ and Jupyter (Lab or Notebook).
- Open the desired `*.ipynb` in the root directory and run cells top-to-bottom.
- For GA/PSO experiments, start with `algo_ga.ipynb`, `algo_ga_4x4.ipynb`, or `algo_pso.ipynb`.

## Suggested Environment

### Python Environment
```bash
python -m venv .venv
.venv/Scripts/activate  # Windows PowerShell: .venv\Scripts\Activate.ps1
pip install jupyter numpy pandas matplotlib 
```
If specific notebooks require extra packages, follow their first code cell or inline notes.

### Gurobi Environment
Check the GuRoBi License, version used in this project is 10.0.2
