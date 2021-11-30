# Noise-Adaptive Compiler Mappings for Noisy Intermediate-Scale Quantum Computers

**Link:** https://arxiv.org/abs/1901.11054

**Authors:**
Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi
**Related:** 


> [time=Fri, May 15, 2020 2:55 PM]
> [name=rum-yasuhiro]
> [color=#0000ff]

###### tags: `Compiler` `NISQ` `Errors in QC` 


[ToC]



<details><summary>Abstruct</summary><div>
A massive gap exists between current quantum computing (QC) prototypes, and the size and scale required for many proposed QC algorithms. Current QC implementations are prone to noise and variability which affect their reliability, and yet with less than 80 quantum bits (qubits) total, they are too resource-constrained to implement error correction. The term Noisy Intermediate-Scale Quantum (NISQ) refers to these current and near-term systems of 1000 qubits or less. Given NISQ's severe resource constraints, low reliability, and high variability in physical characteristics such as coherence time or error rates, it is of pressing importance to map computations onto them in ways that use resources efficiently and maximize the likelihood of successful runs.
This paper proposes and evaluates backend compiler approaches to map and optimize high-level QC programs to execute with high reliability on NISQ systems with diverse hardware characteristics. Our techniques all start from an LLVM intermediate representation of the quantum program (such as would be generated from high-level QC languages like Scaffold) and generate QC executables runnable on the IBM Q public QC machine. We then use this framework to implement and evaluate several optimal and heuristic mapping methods. These methods vary in how they account for the availability of dynamic machine calibration data, the relative importance of various noise parameters, the different possible routing strategies, and the relative importance of compile-time scalability versus runtime success. Using real-system measurements, we show that fine grained spatial and temporal variations in hardware parameters can be exploited to obtain an average 2.9x (and up to 18x) improvement in program success rate over the industry standard IBM Qiskit compiler.
</div></details>



##  Short Summary

calibration-aware compiler techniques for NISQ systemsの提案と評価
> Optimize based on
> - CNOT error rate
> - Readout error rate
> coherence time based も有効ではあるが、current deviceではgate error のインパクトに劣る


<!-- Refs -->


---

## Future works


<!-- Refs -->

---

## Technical Terms

- **LLVM intermediate representation**


<!-- Refs -->


---

## Points of Theory / Technique

SMT approaches

Greedy${\rm V}^\star$, Greedy${\rm E}^\star$
<!-- Refs -->


---

## Results (numerically)


<!-- Refs -->


---


## Next paper


<!-- Refs -->


---
