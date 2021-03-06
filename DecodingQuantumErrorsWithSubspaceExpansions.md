# Decoding quantum errors with subspace expansions

## Information about
**Authors:**
Jarrod R. McClean, Zhang Jiang, Nicholas C. Rubin, Ryan Babbush & Hartmut Neven

**Pub info:**
https://doi.org/10.1038/s41467-020-14341-w

**Funding:**


**Citation**
```
@article{mcclean2020decoding,
  title={Decoding quantum errors with subspace expansions},
  author={McClean, Jarrod R and Jiang, Zhang and Rubin, Nicholas C and Babbush, Ryan and Neven, Hartmut},
  journal={Nature communications},
  volume={11},
  number={1},
  pages={1--9},
  year={2020},
  publisher={Nature Publishing Group}
}
```

## Related papers / repo
- [GeneralizedQuantumSubspaceExpansion](https://github.com/rum-yasuhiro/papers/blob/main/GeneralizedQuantumSubspaceExpansion.md)
- [VirtualDistillationForQuantumErrorMitigation](https://github.com/rum-yasuhiro/papers/blob/main/VirtualDistillationForQuantumErrorMitigation.md)
- [ExponentialErrorSuppressionForNear-TermQuantumDevices](https://github.com/rum-yasuhiro/papers/blob/main/ExponentialErrorSuppressionForNear-TermQuantumDevices.md)
- [IncreasingTheRepresentationAccuracyOfQuantumSimulationsOfChemistryWithoutExtraQuantumResources](https://github.com/rum-yasuhiro/papers/blob/main/IncreasingTheRepresentationAccuracyOfQuantumSimulationsOfChemistryWithoutExtraQuantumResources.md)

## Key Ideas and one paragraph abstraction

### Abstruct
> With rapid developments in quantum hardware comes a push towards the first practical applications. While fully fault-tolerant quantum computers are not yet realized, there may exist intermediate forms of error correction that enable practical applications. In this work, we consider the idea of post-processing error decoders using existing quantum codes, which mitigate errors on logical qubits using post-processing without explicit syndrome measurements or additional qubits beyond the encoding overhead. This greatly simplifies the experimental exploration of quantum codes on real, near-term devices, removing the need for locality of syndromes or fast feed-forward. We develop the theory of the method and demonstrate it on an example with the perfect [[5, 1, 3]] code, which exhibits a pseudo-threshold of p ??? 0.50 under a single qubit depolarizing channel applied to all qubits. We also provide a demonstration of improved performance on an unencoded hydrogen molecule.

### Key ideas

- Using existing quantum error correcting codes to mitigate erros on NISQ
- Styding the performance of these codes under experimental conditions using classical post-processing and addtional measurements
  - mitigate errors on logical qubits using post-processing
  - without explicit syndrome measurements
  - without additional qubits beyond the encoding overhead

## Context

## Technical Terms

- **Stabilizer codes**
  > - Consider a set of n physical qubits.
  > - Quantum error correcting codes utilize entanglement to encode a set of k < n logical qubits, with the hope of improving robustness to probable errors. 
  > - A code that requires at least a weight d Pauli operator to induce a logical error is said to have distance d. 
  > 
  > These three numbers are often used to define a quantum error correcting code, with the notation [[n, k, d]]
  > 
  > $\mathcal{L} = \left\{\bar{X}_{i}, \bar{Z}_{i}\right\}_{i=1, \ldots, k}$
  > 

- **Post-processing**
  > AA

- **Quantum Subspace Expansion**
  > AA


- **perfect code**
  > [[n, k, d]] = [[5, 1, 3]]

- **XX**
  > AA

## Data

## Impact

