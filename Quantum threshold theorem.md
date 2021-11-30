# Quantum threshold theorem

**Related notes**: 
- [Fault-tolerant quantum computation with long-range correlated noise](https://github.com/rum-yasuhiro/papers/blob/main/Fault-tolerant%20quantum%20computation%20with%20long-range%20correlated%20noise.md#fault-tolerant-quantum-computation-with-long-range-correlated-noise)
- [Sufficient condition on noise correlations for scalable quantum computing](https://github.com/rum-yasuhiro/papers/blob/main/Sufficient%20condition%20on%20noise%20correlations%20for%20scalable%20quantum%20computing.md#sufficient-condition-on-noise-correlations-for-scalable-quantum-computing)


**papers**
- [Quantum accuracy threshold for concatenated distance-3 codes](https://arxiv.org/abs/quant-ph/0504218)
- [Fault-tolerance threshold for a distance-three quantum code](https://arxiv.org/abs/quant-ph/0509203)


> [time=Fri, Jun 5, 2020 11:17 AM] 
> rum
> [color=#0000ff]

###### tags: `Error Correction` `Quantum threshold theorem`

[ToC]

## Fault-torelant quantum computation(フォールトトレラント量子計算)

### noise and decoherence
### error correction code


## threshold theorem(閾値定理)

> "The entire content of the Threshold Theorem is that you're correcting errors faster than they're created. That's the whole point, and the whole non-trivial thing that the theorem shows. That's the problem it solves."[3]
> [Scott Aaronson](https://en.wikipedia.org/wiki/Scott_Aaronson)

> しきい値定理とは、「量子ゲートで発生するエラーの確率がある値（誤りしきい値= noise threshold）よりも小さければ効率よく（多項式時間で）任意の精度で量子計算を実行できる」ということである。
> このしきい値定理の証明には、有限サイズの量子誤り訂正符号を階層化した連接量子符号（concatenated quantum code）による連接量子計算（concatenated quantum computation）が用いられる。近年、連接量子計算とはことなった方法である、トポロジカル符号を用いたトポロジカルフォールトトレラント量子計算も提案されている。[フォールトトレラント量子計算 wiki]

### Technical terms

- independent stochastic faults model
	> faults are independently and identically distributed at the locations of the noisy quantum circuit
	> at each location either the gate is executed perfectly (with probability 1−ε), or a fault occurs (with probability ε)
	> ε: fault rate
	> Though the fault locations are chosen probabilistically, once the locations are chosen the action of the faulty gates can be chosen adversarially
	> つまり、we allow the faults to be arbitrary trace-preserving quantum operations.


- trace-preserving quantum operations

### Threshold theoremが想定するエラーとその大きさ

| paper | Gate error | bath | correlated | stochastic noise model | 
| ----- | ---------- | ---- | ---------- | --- |
|[PAN 05][QUANTUM ACCURACY THRESHOLD FOR CONCATENATED DISTANCE-3 CODES]| ||| $\epsilon \leq 2.73 \times 10^{-5}$ |
||||||

### accuracy threshold
It is the noise threshold so that quantum computation can be executed with high reliability.

$\epsilon \leq 2.73 \times 10^{-5}$ for adversarial independent stochastic noise model
> [QUANTUM ACCURACY THRESHOLD FOR CONCATENATED DISTANCE-3 CODES]





<!-- Refs -->
[3]: https://www.scottaaronson.com/democritus/lec14.html
[フォールトトレラント量子計算 wiki]:https://ja.wikipedia.org/wiki/%E3%83%95%E3%82%A9%E3%83%BC%E3%83%AB%E3%83%88%E3%83%88%E3%83%AC%E3%83%A9%E3%83%B3%E3%83%88%E9%87%8F%E5%AD%90%E8%A8%88%E7%AE%97

[QUANTUM ACCURACY THRESHOLD FOR CONCATENATED DISTANCE-3 CODES]: https://arxiv.org/abs/quant-ph/0504218

---
