# Mapping of quantum circuits onto NISQ superconducting processors

### Authers
Lingling Lao,1 Daniel M. Manzano,2 Hans van Someren,1 Imran Ashraf,1 and Carmen G. Almudever


> 2020 / 04 / 07
> 
> [color=#0000ff]

###### tags: `Compiler`　`Router` `NISQ` `Suerface-17` `IBMQ` `Fault-tolerance` 

[ToC]

Related notes:

- [Assessing the mapping of quantum algorithms](/G7aGKZw_TbW5ND4NmQFn2g?both)
- [Challenges and Opportunities of Near-Term Quantum Computing Systems](/9Y8XSNnfScaqlGeiNirCVw)
- 

## Short summary

NISQ向けの**Qmap**と呼ばれるmapper に関する論文

デバイスのelementary gate set や connectivity だけでなく、
classical control の観点についてもカバーしているところが新しい

**Qmap**は[**OpenQL**]のコンパイラに組み込まれている。

<!-- Refs -->
[Mapping of quantum circuits onto NISQ superconducting processors]:https://arxiv.org/abs/1908.04226
[**OpenQL**]: http://openql.org/

---

## 用語

**Compiler**
- **mapper**
    > hardware-agnostic circuit :arrow_right: harware-aware circuit
    > [color=#0000ff]

- **initial placement**
- **routing**
    > virtual qubits をcxなどのオペレーションで関係するnon-adjacent qubits 同士を隣接するように動かすこと
    > - **shuttling**: trapped ion と Si-spin 方式の量子プロセッサにおけるSWAPのような作用
    > [color=#aaff00]
    - **minextendrc**: 本論文で紹介されている3つのrouting strategiesのうちの一つ (trivual, base and minextendrc)


- operation scheduling
- gate decomposition and optimization

Classical control
> qubit操作に用いらるclassical electronics
個々のqubitに対してdedicated instrumentを用いるのはコストが高いので、プロセッサをスケールさせるためにもshared controlが用いられる。ただし、latencyやdepthが大きくなることからparallelismの障壁となる。
>[color=#ff00f0]
- AWG ( Arbitrary Wave form Generator )
    > operating on a group of qubits
    > 同じfeedlineで測定される
    > [color=#ff0000]
:::info
プロセッサーがスケールしていったときに、classical controlの影響は非常に効いてくる。
:::

**hardware-agnostic**: ハードウェアに依存しない
> :left_right_arrow: hardware-aware

**ESP( execution success rate)**




<!-- Refs -->


---

## 重要な技術、理論

**Qmap** :desktop_computer: 
> - [x] it considers not only *gate set* *connectivity* but also *classical control*
> - [x] for supporting several quantum processors, it has been embedded in OpenQL compiler
> - [x] mapper supports different routing strategies (trivial, base and minextendrc)
> - [x] it uses not only SWAP but also MOVE (2 CNOTs) when possible
> [color=#ffff00]




<!-- Refs -->


---


##  Future work

- より多くのqubitを含むmapping
- initial placement and routing
    - finding movement operation for several two-qubit gates simultaneously
- より多くのmapping metricsについて調査し組み込む
- 現状 mapping based on gate level だが、[microarchitecture]に対する手法とも比較
    - pulse levelでのコンパイル手法との比較 (trade-off)を示す


<!-- Refs -->
[microarchitecture]: https://dl.acm.org/doi/10.1145/3123939.3123952

---


## 次に読むべき

- [Assessing the mapping of quantum algorithms](/G7aGKZw_TbW5ND4NmQFn2g)
- [An experimental microarchitecture for a superconducting quantum processor]
- [Challenges and Opportunities of Near-Term Quantum Computing Systems]
- [QLib: Quantum module library]

<!-- Refs -->
[An experimental microarchitecture for a superconducting quantum processor]:https://dl.acm.org/doi/10.1145/3123939.3123952
[QLib: Quantum module library]: https://dl.acm.org/doi/10.1145/2629430
[Challenges and Opportunities of Near-Term Quantum Computing Systems]:https://arxiv.org/abs/1910.02894

---
