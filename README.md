# Lab: Foundations of Neural Networks (1943–1960)

This lab explores the origins of Connectionism and Artificial Intelligence through the implementation and analysis of four seminal models. You will move from hard-coded logic with McCulloch-Pitts neurons to the birth of supervised gradient descent with ADALINE.

## 📂 Table of Contents

1. [Part 1: McCulloch-Pitts Neuron](https://www.google.com/search?q=%23part-1-mcculloch-pitts-neuron)
2. [Part 2: Hebbian Learning & Oja's Rule](https://www.google.com/search?q=%23part-2-hebbian-learning--ojas-rule)
3. [Part 3: The Rosenblatt Perceptron](https://www.google.com/search?q=%23part-3-the-rosenblatt-perceptron)
4. [Part 4: ADALINE & Gradient Descent](https://www.google.com/search?q=%23part-4-adaline--gradient-descent)

---

## 🧠 Part 1: McCulloch-Pitts Neuron (1943)

The earliest computational model of a biological neuron. This section focuses on propositional logic and the "all-or-nothing" thresholding mechanism.

* **Logic Synthesis:** Implement AND, OR, NOT, NAND, and NOR gates using fixed weights and thresholds.
* **The XOR Problem:** Mathematically demonstrate why a single M-P neuron cannot solve the XOR problem (linear inseparability).
* **Network Architectures:** Build a 3-neuron feedforward network to successfully solve XOR.
* **Visualization:** Plot the 2D decision boundaries to see the linear separation of logic classes.

---

## 🧬 Part 2: Hebb's Rule (1949)

"Neurons that fire together, wire together." This part explores unsupervised learning and biological plasticity.

* **Correlation Learning:** Implement basic Hebbian learning ($w_i = w_i + \eta x_i y$) and observe how weights grow to represent data clusters.
* **The Divergence Problem:** Analyze why standard Hebbian learning leads to infinite weight growth.
* **Oja's Rule:** Implement the normalized Hebbian update to stabilize weights and perform **Principal Component Analysis (PCA)**.
* **Associative Memory:** Create a simple memory system that retrieves patterns based on correlations.

---

## ⚖️ Part 3: Perceptron (1957)

Frank Rosenblatt’s Perceptron introduced the first supervised learning algorithm with an explicit error-correction rule.

* **Learning Rule:** Implement the Perceptron update: $w \leftarrow w + \eta(y - \hat{y})x$.
* **Linear Separability:** Test the algorithm on the Iris dataset and logic gates.
* **Optimization:** Analyze the impact of the **Learning Rate ($\eta$)** and the order of training data on convergence speed.
* **Advanced Variants:** Implement a **Voting Perceptron** to improve generalization and compare results against `scikit-learn`.

---

## 📉 Part 4: ADALINE (1960)

The **ADA**ptive **LI**near **NE**uron introduced the use of a continuous linear activation function and the Mean Square Error (MSE) loss function.

* **Gradient Descent:** Implement the Delta Rule (Widrow-Hoff) to minimize cost via the surface gradient.
* **Optimization Strategies:**
* **Batch:** Calculate gradients over the entire dataset.
* **Stochastic (SGD):** Update weights after every single sample.
* **Mini-batch:** The modern middle ground for efficiency.


* **Data Preprocessing:** Demonstrate why feature standardization (scaling) is critical for gradient descent convergence.
* **Extensions:** Implement **Momentum** and **Learning Rate Decay** to navigate the loss landscape more effectively.
