# Variational Quantum Attack on Symmetric-Key Ciphers

**Authors**: Kurella Anand Kasyup (EP22BTECH11012), Edara Yaswanth Balaji (EP22BTECH11007)

**Affiliation**: Department of Physics, Indian Institute of Technology Hyderabad

---

This repository hosts the detailed documentation for our semester project on applying Variational Quantum Attack Algorithms (VQAA) to attack simplified DES (S‑DES) ciphers. All code implementations have been omitted; here you will find project descriptions, theoretical background, experimental workflows, results, and visual summaries.

## Contents

```
├── docs/
│   ├── VQAA_Semester_Project_Report.pdf        # Full project report with formulations, methods, and results
│   ├── Poster.pdf                              # Conference‑style poster summarizing key findings
│   └── Quantum_Attacks_for_Symmetric_Crypto_Systems.pdf  # Slide deck and supplementary explanations
├── LICENSE                                     # MIT License
├── .gitignore                                  # Ignore temporary and system files
└── README.md                                   # This overview document
```

## Project Overview

* **Objective**: Demonstrate how variational quantum circuits can be used to recover S‑DES keys via cost‑minimization strategies in Qiskit.
* **Approach**:

  1. Formalize the S‑DES encryption/decryption as a parameterized Hamiltonian.
  2. Design an ansatz circuit (U–CNOT layers) whose parameters encode candidate keys.
  3. Define a cost function measuring Hamming distance between observed ciphertext and circuit output.
  4. Use a classical optimizer (COBYLA, SPSA) to minimize the cost and identify the secret key.
* **Results**:

  * Convergence curves for baseline vs. improved ansatz.
  * Statistical histograms over multiple runs showing success rates.
  * Analysis of optimizer sensitivity and noise resilience.

## How to Explore

1. **Read the full report** (`docs/VQAA_Semester_Project_Report.pdf`):

   * Background on S‑DES and variational algorithms.
   * Mathematical derivations (Hamiltonian construction, cost landscapes).
   * Detailed explanation of circuit design and optimization loops.
   * Tabulated and graphical results with discussions.

2. **View the poster** (`docs/Poster.pdf`):

   * Visual summary of methodology and key outcomes.
   * High‑level figures and take‑home messages.

3. **Open the slides** (`docs/Quantum_Attacks_for_Symmetric_Crypto_Systems.pdf`):

   * Slide‑by‑slide walkthrough of theory, experiments, and conclusions.
   * Supplementary diagrams and parameter tables.

## License

This work is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

*For questions or clarifications, please contact the authors via email (see report cover page).*
