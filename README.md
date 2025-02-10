# Shor's Algorithm
Implementation of Shor's algorithm using unitary matrices and Qiskit.

## 📖 Overview
This project presents an implementation of Shor's Algorithm, a quantum algorithm for integer factorization, using Qiskit. Shor’s algorithm leverages quantum parallelism to efficiently find the prime factors of large numbers, demonstrating the power of quantum computing over classical methods for certain problems.

## 🧑‍🏫 About the Project
Course: Quantum Computation
Institution: Universidad Politécnica de Madrid
Objective: To explore quantum algorithms and their advantages over classical approaches by implementing Shor’s algorithm using Qiskit.

## ⚙️ Features
Simulates Shor’s algorithm on a quantum circuit.
Uses Quantum Fourier Transform (QFT) for period finding.
Implements modular exponentiation efficiently within Qiskit.

## 🛠 Installation & Dependencies

Ensure you have Python installed, then install Qiskit along with its required components:  

```bash
pip install qiskit qiskit-aer qiskit-ibm-runtime qiskit[visualization]
```
## 📜 How Shor's Algorithm Works

1. **Choose an integer N** (the number to factor).  
2. **Select a random integer a** such that \(1 < a < N\).  
3. **Check if** \(\gcd(a, N) \neq 1\). If true, we have found a factor.  
4. **Use quantum computing to find the period** \( r \) of the function:  
   \[
   f(x) = a^x \mod N
   \]
5. **Determine the factors** of \( N \) using:  
   \[
   \gcd(a^{r/2} - 1, N)
   \]

## 📌 Limitations
Quantum simulators can only handle small numbers due to hardware constraints.
Running the algorithm on real quantum hardware is challenging due to noise and decoherence.

## 🏗 Future Improvements
Optimize modular exponentiation for better efficiency.
Test on real quantum hardware using IBM Quantum Experience.
Explore error mitigation techniques.

## 📝 References
Shor, P. W. (1994). Algorithms for quantum computation: discrete logarithms and factoring.
Scott Aaronson (2018). Introduction to Quantum Information Science Lecture Notes
Qiskit Documentation: https://qiskit.org/documentation/

## 🤝 Contributing
Feel free to submit issues or contribute improvements via pull requests.



