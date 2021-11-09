# Distributing Multipartite Entanglement over Noisy Quantum Networks

## Information about
- Authors: 
  > Luís Bugalho, Bruno C. Coutinho, Francisco A. Monteiro, Yasser Omar
- Pub info:
  > arXiv:2103.14759 [quant-ph]
- Funding:
  > 

## Key Ideas and one paragraph abstraction
They propose an algorithm for generating multipartite entanglement on noisy network.
This is optimal for GHZ states with 3 qubits, maximising fidelity and rate of entanglement distribution.
Also provide adaptability for the system with higher number of qubits and other types of multipartite entanglement.


### Abstruct
> A quantum internet aims at harnessing networked quantum technologies, namely by distributing bipartite entanglement between distant nodes. However, multipartite entanglement between the nodes may empower the quantum internet for additional or better applications for communications, sensing, and computation. In this work, we present an algorithm for generating multipartite entanglement between different nodes of a quantum network with noisy quantum repeaters and imperfect quantum memories, where the links are entangled pairs. Our algorithm is optimal for GHZ states with 3 qubits, maximising simultaneously the final state fidelity and the rate of entanglement distribution. Furthermore, we determine the conditions yielding this simultaneous optimality for GHZ states with a higher number of qubits, and for other types of multipartite entanglement. Our algorithm is general also in the sense that it can optimise simultaneously arbitrary parameters. This work opens the way to optimally generate multipartite quantum correlations over noisy quantum networks, an important resource for distributed quantum technologies.

### Key ideas
- rate of distribution
- the final state fidelity



## Context

### Quantum Network

<img width="538" alt="Screen Shot 2021-11-09 at 9 44 32" src="https://user-images.githubusercontent.com/42485819/140840965-479e56cb-c110-4792-95d0-e046c14e2133.png">

> FIG. 1. (a) Star composed by 3 different paths, connecting terminal nodes τ , η and θ to the center node c. Notice that the rate ξtree depends on each branch probability of success pc:τ and communications time tc:τ (Eq. 2). Moreover, the fidelity of the final state ftree depends on each branch fidelity Fc:τ (Eq. 3).
> (b) Branch composed by an arbitrary number of links. Each branch final fidelity Fc:τ depends on the path values γi:j , communications time ti:j , and memory decoherence times σi:j . The probability of success pc:τ depends on each link probability pi:j and the entanglement swapping probabilities kj . The communications time tc:τ depends on the lengths and the velocity of light Li:j/c.

## Technical Terms
- **Multipartite entanglement**
  > AA
- **GHZ state**
  > AA
- **Quantum repeater**
  > AA
- **Werner state**
  > $\rho_{W}=\gamma\left|\phi^{+}\right\rangle\left\langle\phi^{+}\right|+(1-\gamma) \mathbb{1}$
  > 
  > where $\gamma=(4 F-1) / 3$
  > 
  > and F is the [fidelity](https://en.wikipedia.org/wiki/Fidelity_of_quantum_states).
- **[Depolarising channel](https://en.wikipedia.org/wiki/Quantum_depolarizing_channel)**
  > $\begin{aligned}
\mathcal{D}_{i}^{p}(\rho) &=p \rho+\frac{1-p}{3}\left(\hat{X}_{i} \rho \hat{X}_{i}^{\dagger}+\hat{Y}_{i} \rho \hat{Y}_{i}^{\dagger}+\hat{Z}_{i} \rho \hat{Z}_{i}^{\dagger}\right) \\
&=\frac{1+2 p}{3} \rho+\frac{2(1-p)}{3} \Lambda_{i}\left(\hat{Y}_{i} \rho \hat{Y}_{i}^{\dagger}\right)
\end{aligned}
  > 
  > In the bipartite case, there is an equivalence between a Werner state and a representation with a depolarising channel having an equal amount of bit-flip, phase-flip and phase-bit-flip errors:
  >
  >  \rho_{W}=\mathcal{D}_{1}^{F}\left(\left|\phi^{+}\right\rangle\left\langle\phi^{+}\right|\right)=\mathcal{D}_{2}^{F}\left(\left|\phi^{+}\right\rangle\left\langle\phi^{+}\right|\right)
  > 
- **Steiner tree**
  > AA


- **XX**
  > AA


## Data
<img width="1329" alt="Screen Shot 2021-11-09 at 9 48 06" src="https://user-images.githubusercontent.com/42485819/140841286-f6051459-35aa-429c-a02c-bb423332783c.png">

<img width="1404" alt="Screen Shot 2021-11-09 at 9 48 25" src="https://user-images.githubusercontent.com/42485819/140841309-bdd739a4-e317-4408-9bfb-b7f05ab2ba19.png">

> FIG. 3. Simulations for MOSP algorithm and Algorithm 1 for 3 and 4 qubits GHZ state distribution in (b) Erd¨os-R´enyi networks with average degree $\langle\lambda\rangle=3$ and (d) random geometric networks with average degree $\langle\lambda\rangle=8$, displaying as well the average number of solutions found for Algorithm 1
applied to the 3-qubits problem in (a) Erd¨os-R´enyi networks and (c) random geometric networks. The parameters utilized are:
> $p_{\min }=0.5$, 
> $t_{\min }=1$, 
> $t_{\max }=100$, 
> $\sigma_{\min }=10^{4}$, 
> $\sigma_{\max }=10^{5}$, 
> $f_{\text {trunc }}^{\mathrm{GHZ}}=0.5$, 
> $f_{\text {trunc }}^{\text {path }}=0.9$.
> For a Erd¨os-R´enyi network $a = 2$ and 
> d_{\max }=\log N / \log \langle\lambda\rangle [42, 43]. 
> For random geometric networks $a = 2$ and $d_{\max }=\sqrt{N / \log N}$ [44].

## Impact
- This methodology can be applied
  - different distribution scheme
  - different quantum repeater protocols 
- While optimality is not always the practical goal, this tool can be utilize as a measure to find a closeness to optimality and possibility new routing protocols that are close to optimal.



## Related papers / repo


