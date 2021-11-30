# Optimal Layout Synthesis for Quantum Computing

**Link:**
https://arxiv.org/abs/2007.15671

**Authors:**
Bochen Tan, Jason Cong

**Related:** 


> [time=Thu, Sep 24, 2020 11:31 AM]
> rum
> [color=#0000ff]

###### tags: `Compiler` `Router` 


[ToC]



<details><summary>Abstruct</summary><div>
Recent years have witnessed the fast development of quantum computing. Researchers around the world are eager to run larger and larger quantum algorithms that promise speedups impossible to any classical algorithm. However, the available quantum computers are still volatile and error-prone. Thus, layout synthesis, which transforms quantum programs to meet these hardware limitations, is a crucial step in the realization of quantum computing. In this paper, we present two synthesizers, one optimal and one approximate but nearly optimal. Although a few optimal approaches to this problem have been published, our optimal synthesizer explores a larger solution space, thus is optimal in a stronger sense. In addition, it reduces time and space complexity exponentially compared to some leading optimal approaches. The key to this success is a more efficient spacetime-based variable encoding of the layout synthesis problem as a mathematical programming problem. By slightly changing our formulation, we arrive at an approximate synthesizer that is even more efficient and outperforms some leading heuristic approaches, in terms of additional gate cost, by up to 100%, and also fidelity by up to 10x on a comprehensive set of benchmark programs and architectures. For a specific family of quantum programs named QAOA, which is deemed to be a promising application for near-term quantum computers, we further adjust the approximate synthesizer by taking commutation into consideration, achieving up to 75% reduction in depth and up to 65% reduction in additional cost compared to the tool used in a leading QAOA study.
</div></details>



##  Short Summary
layout synthesisに関する提案
- Optimal
    exact layout synthesizer (OLSQ)
- Approximate
    approximate, transition based synthesizer(TB-OLSQ)
    - additional gate cost: up to 100%
    - Fidelity: up to 10x
- QAOA 
    TB-OLSQ for QAOA (QAOA-OLSQ)


<!-- Refs -->


---

## Future works
- correlated errorを含めた手法
- commutation relations, special stucture inside the grph(coupling graph)を含めたsynthesizerの開発
- 

<!-- Refs -->

---

## Which theory / technique is criticized?


<!-- Refs -->

---


## Technical Terms
Architecture and design automation for quantum computing

Time and Space coodinates in Quantum circuit


QUEKO (Quantum mapping example with known optimal)

<!-- Refs -->


---

## Points of Theory / Technique

### Formulation



<!-- Refs -->


---

## Results (numerically)


<!-- Refs -->


---


## Next paper
Matteo G. Pozzi, Steven J. Herbertらの論文
- [Using Reinforcement Learning to Perform Qubit Routing in Quantum Compilers](https://arxiv.org/abs/2007.15957)

CQC の t ket の論文
- [t|ket⟩ : A Retargetable Compiler for NISQ Devices](https://arxiv.org/abs/2003.10611)


Optimal layout synthesis
- [Qubit allocation](https://dl.acm.org/doi/abs/10.1145/3168822)
- [MUQUT: Multi-Constraint Quantum Circuit Mapping on NISQ Computers: Invited Paper](https://ieeexplore.ieee.org/document/8942132)
- [Mapping Quantum Circuits to IBM QX Architectures Using the Minimal Number of SWAP and H Operations
](https://arxiv.org/abs/1907.02026)

<!-- Refs -->


---
