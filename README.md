# COIT29224 Evolutionary Computation - Assignment 2 Example
## Optimization with (1+1)-Evolution Strategy

This repository contains a Python implementation of a (1+1)-Evolution Strategy (ES) with the 1/5th success rule for mutation strength adaptation. The ES is applied to optimize a complex, 2D multi-modal objective function (a modified Easom function).

### Objective Function

The function to be minimized is:
`f(x, y) = -cos(x) * cos(y) * exp(-((x - π)^2 + (y - π)^2)) + 0.01 * ((x - 2)^2 + (y + 1)^2)`
The search is conducted within the bounds `x, y ∈ [-5, 5]`. The global minimum is expected near `(π, π)`.

### Files

*   `run_es_complex.py`: The main Python script containing the ES implementation and plotting logic.
*   `requirements.txt`: Python package dependencies.
*   `fitness_sigma_convergence.png`: Saved plot of fitness and sigma convergence.
*   `search_path_contour.png`: Saved plot of the ES search path on the function landscape.

### How to Run

1.  **Clone the repository:**
    ```bash
    git clone <your_repository_url>
    cd <repository_name>
    ```
2.  **Set up a Python environment:**
    It's recommended to use a virtual environment.
    ```bash
    python -m venv es_env
    source es_env/bin/activate  # On Windows: es_env\Scripts\activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Run the script:**
    ```bash
    python run_es_complex.py
    ```
    This will execute the (1+1)-ES, print progress and final results to the console, and generate/save two plots: `fitness_sigma_convergence.png` and `search_path_contour.png`.

### Report
The `REPORT.md` file contains the detailed write-up of the project, including problem formulation, ES implementation details, results, analysis, discussion, and conclusions, structured to meet the assignment criteria. (You would replace this sentence with a link to the actual PDF if you convert it).
