# Generating Fault-Tolerant Cluster States from Crystal Structures

Michael Newman
Leonardo Andreta de Castro
Kenneth R. Brown

> 2020 / 3 / 2
> 
> [color=#0000ff]

###### tags: `MBQC` `Cluster state` `Fault-tolerance` `Error Correction` 

[ToC]

## アブスト

fault-tolerant cluster states derived from crystal structures

結晶構造によるフォルトトレラントなcluster状態を構築する理論を提案。
combinatorial tiling theoryという理論に基づいている。

**robust self-dual cluster state**: 次数３でできるcluster state


<!-- Refs -->


---

## 要素技術、用語

### **foliation**(葉)
文字通り、


### Fault-tolerant cluster state

#### Quantum CSS codes


**chain complex** $C$ :  a sequence of vector space $\{ C_{i} \}$
**boundaries** $\{ \partial_{i} \}$ : liner maps between chain complex $C$: 

$$
0 \rightarrow
C_l \xrightarrow{\partial_l}
C_{l-1} \rightarrow
\dots \rightarrow
C_{1} \xrightarrow{\partial_1} 
C_{0} \rightarrow 
0
$$


**coboundaries** $\{ \partial_{i} \}$ : liner maps between chain complex $C^*$: 

$$
0 \leftarrow
C^l \xleftarrow{\partial^l}
C^{l-1} \leftarrow
\dots \leftarrow
C^{1} \xleftarrow{\partial^1} 
C^{0} \leftarrow 
0
$$

#### Fault-tolerant cluster states as chain complexes

*graph state* $\vert G \rangle$ is the unique state stabilized by the set of operators 

$$
\{ X_{v} \ \Pi \ Z_{w}: v \in V \}
$$

:::info
A *fault-tolerant cluster state* can be identified with a length-3 chain complex $C$: 

$$
C_{3} \xrightarrow{\partial_{3}}
C_{2} \xrightarrow{\partial_{2}}
C_{1} \xrightarrow{\partial_{1}}
C_{0}
$$
:::

$C_{1} : primal$
$C_{2} : dual$


#### Circuit-based error model and its effects

consider three types of errors: 
- SPAM errors with probability $p_m$
- X-type errors occur on the **dual** qubit support of a CZ gate with probability $p_X$ after the gate.
- Z-type errors occur on the **primal** qubit support of a CZ gate with probability $p_Z$ after the gate.


<!-- Refs -->


---

##  


<!-- Refs -->


---


## 次に読むべき論文

- [Universal fault-tolerant measurement-based quantum computation]




<!-- Refs -->

[Universal fault-tolerant measurement-based quantum computation]: https://arxiv.org/abs/1811.11780

---


## Citation

```tex
@misc{newman2019generating,
    title={Generating Fault-Tolerant Cluster States from Crystal Structures},
    author={Michael Newman and Leonardo Andreta de Castro and Kenneth R. Brown},
    year={2019},
    eprint={1909.11817},
    archivePrefix={arXiv},
    primaryClass={quant-ph}
}

```
