# CertiQ: A Mostly-automated Verification of a Realistic Quantum Compiler

Authors: 
Yunong Shi, Xupeng Li, Runzhou Tao, Ali Javadi-Abhari, Andrew W. Cross, Frederic T. Chong, Ronghui Gu

> 2020 / 04 / 29
> rum
> [color=#0000ff]

**Link**
https://arxiv.org/abs/1908.08963

###### tags: `Compiler` `Qiskit` `NISQ`


[ToC]

<details><summary>Abstruct</summary><div>
In this paper, we present CertiQ, a mostly-automated verification framework for the Qiskit quantum compiler. To our knowledge, CertiQ is the first effort to apply formal verification and SMT reasoning to a real-world quantum compiler. Qiskit is currently the most complete and widely-used open-source quantum software stack from low-level compilation to high-level quantum algorithms. With growing community contributions, the Qiskit compiler is in need of code quality control and verification down to the compilation level to guarantee reliability of scientific work that uses it. CertiQ is deeply integrated into the Qiskit compiler (called Terra), providing abstract specifications for quantum compiler data structures and offering verifiable contracts that specify the behaviors of compilation phases with heavy optimizations. CertiQ enables verification of the existing implementation of the Qiskit compiler and future code submissions in a mostly-automated manner using invariant-guided contracts and contract continuation. With these techniques in place, developers need to provide limited inputs only where function contracts and loop invariant cannot be inferred automatically. The CertiQ verification procedure discovers several critical bugs, some of which are unique to quantum soft-ware. Our extensive case studies on four compiler phases of Qiskit demonstrate that CertiQ is effective for verification of quantum compilers with a low proof burden.
</div></details>


##  Short Summary
Qiskit コンパイラのための　mostly-automated verification framework： **CertiQ**

CertiQ は quantum software 特有のバグを検出できることを示した

<!-- Refs -->

---

## Future works
この contract-based approach を Aqua や Openpulse など、様々な階層に組み込む

<!-- Refs -->

---

## Technical Terms
- **SMT reasoning**

- **contract-based design**

- **invariant contract**


<!-- Refs -->


---

## Points of Theory / Technique


<!-- Refs -->


---

## Results (numerically)


<!-- Refs -->


---


## Next paper


<!-- Refs -->


---
