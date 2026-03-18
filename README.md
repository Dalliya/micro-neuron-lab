# 🧠 Neural Network Forward Pass: Matrix Inference Visualizer

## 📖 Abstract

Welcome to my specialized visualization environment designed to demystify the **forward pass mechanics** of a neural network. Moving beyond abstract mathematical notation, this project maps precise matrix operations (weighted sums) directly onto a continuously differentiable activation space (the Sigmoid curve). 

To make the learning process both engaging and visually striking, the entire mathematical pipeline is wrapped in a custom, procedurally generated "Matrix" cyberpunk aesthetic using pure Python.

## 🔬 Methodology & Inspiration

The mathematical foundation and pedagogical approach of this project are heavily inspired by **Tariq Rashid's** excellent book, *"Make Your Own Neural Network"*. 

Following Rashid's core philosophy of "understanding the matrix math under the hood," I developed this visualization to explicitly show the transition from discrete inputs and synaptic weights to the final continuous output. By manually calculating the weighted sums and mapping them to their precise activation thresholds, this project bridges the gap between abstract calculus and geometric intuition.

## 🧮 Core Architecture & Mathematics

Instead of relying on random number generation, this visualizer uses explicit, hardcoded parameters to prove the mathematical concept:

1. **Inference State:** Precise modeling of a 2-node hidden layer forward pass.
   * **Inputs (I):** $[0.5, 1.0]$
   * **Weights (W):** $\begin{bmatrix} 0.3 & 0.2 \\ 0.9 & 0.5 \end{bmatrix}$
   * **Weighted Sums (X):** $X_1 = 0.35$, $X_2 = 0.95$
2. **Activation Function:** Application of the standard logistic sigmoid function using `scipy`: $\sigma(x) = \frac{1}{1 + e^{-x}}$
   * **Final Outputs (Y):** $Y_1 \approx 0.5866$, $Y_2 \approx 0.7211$
3. **Visual Engine:** A custom Matplotlib rendering pipeline featuring:
   * Procedurally generated, fading binary code rain (`#00ff41`).
   * Collision-proof, mathematically annotated data points using high-contrast neon mapping (Cyan & Magenta).
   * An integrated "telemetry dashboard" displaying the real-time matrix math.

## 🚀 Quick Start / Reproduction

To explore this visualization and the underlying matrix math:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/nn-forward-pass-viz.git](https://github.com/yourusername/nn-forward-pass-viz.git)
   cd nn-forward-pass-viz
Install the dependencies:

Bash
pip install numpy scipy matplotlib jupyter
Launch the Notebook:
Open solution.ipynb in VS Code, Jupyter Notebook, or Google Colab to execute the cells and interact with the visualization environment.

Note: The script will automatically generate and save a high-resolution matrix_plot.png file in your directory upon execution.

📸 Experimental Results
(Fig 1. Geometric mapping of hidden layer neuron activations plotted against the global sigmoid space. Generated natively via Matplotlib).

👩‍💻 Author & Contribution
This research, the mathematical calculations, and the custom visualization logic were developed entirely by Dariia Zhdanova.

This project serves as a comprehensive demonstration of translating theoretical mathematics (as outlined by Tariq Rashid) into a functional, high-fidelity digital asset.

Developed by Dariia Zhdanova | 2026 | Neural Network Research Series ```