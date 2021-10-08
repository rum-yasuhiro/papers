# Using Reinforcement Learning to Perform Qubit Routing in Quantum Compilers

## Information about
- Authors: 
  > Matteo G. Pozzi (1), Steven J. Herbert (1 and 2), Akash Sengupta (3), Robert D. Mullins (1) ((1) University of Cambridge Computer Laboratory, (2) Cambridge Quantum Computing, (3) Department of Engineering, University of Cambridge)
- Pub info:
  > https://arxiv.org/abs/2007.15957
- Funding:
  > 

## Key Ideas and one paragraph abstraction

### Abstruct
> "Qubit routing" refers to the task of modifying quantum circuits so that they satisfy the connectivity constraints of a target quantum computer. This involves inserting SWAP gates into the circuit so that the logical gates only ever occur between adjacent physical qubits. The goal is to minimise the circuit depth added by the SWAP gates. In this paper, we propose a qubit routing procedure that uses a modified version of the deep Q-learning paradigm. The system is able to outperform the qubit routing procedures from two of the most advanced quantum compilers currently available, on both random and realistic circuits, across near-term architecture sizes.

### Key ideas
- 強化学習(DQN)でルーティング
- Herbert and Senguptaの先行研究を改良 [[HER 18]]
> - This proposed RL formulation addressed the optimization of duration time of each gate.
> 
- near-term architecture sizeにrandom circuitで他を凌駕


## Context
- action space is combinatorial: possible parallelisable sets of SWAP are $\mathcal{O}(2^n)$. 
    > Instead learining the quality of individual state and combinationatorial optimisation technique, search for the action leading to the highest-quality next stage. 
    > 
- 

## Technique
- The quality function
    $Q(s)=r^{\*}(s)+\gamma \max \_ {a} Q(\operatorname{env}(s, a))$
    > 
## Technical Terms
### Qubit routing
    > the task of modifying quantum circuits so that they satisfy the connectivity constraints of a target quantum computer.
    > They involves inserting SWAP gate into the circuit so that the logial gates only ever occure between adjacent physical qubits. 
    > The goal is to minimise the circuit depth added by the SWAP gates.
    > 

### Reinforcement Learning
- State
    > プロセッサと量子回路の実行具合
    > N: 物理ノード
    > Q: 論理量子ビット(logical qubits)
    > Qubit location: N-->Q
    > Qubit targets: Q-->Q
    > Circuit progress Q --> $N_{d+1}$
- Reword
    > 報酬が出されるタイミング
    > - ゲートスケジュール時
    > - 
- Action 
    > 並列で実行できるSWAPのセット
    > Action space: O(2^n) possible parallelisable sets of SWAP to choose from.
    > 個々のstateの質を学習し、組み合わせ最適化手法(simulated annealing)で最もfidelityの高くなるSWAPの差し込み方を探索する

### Q-Learning model
- Quality function: 
> Q(s)=r^{*}(s)+\gamma \max _{a} Q(\operatorname{env}(s, a))
> r^{*}が方策に則り報酬を出す

- model
> Q\left(s_{t}\right) \leftarrow(1-\alpha) Q\left(s_{t}\right)+\alpha\left(r_{t}+\gamma \max _{a_{t+1}} Q\left(s_{t+1}\right)\right)
> 
> \left(s t, a_{t}, r_{t}, s_{t+1}\right)

### Learning process

Utilized following two techniechs to enhance deep Q-learning

- Double Deep Q-learning (DDQN)
> Improve the statbility of the learning process by useing two neural networks instead of one.
- Prioritised Experience Replay
> Enhance the learning process by replaying more useful experiences with a higher priority.

### Qubit routing with Q-learning

RL formulation don't provide timestep problem to minimize circuit depth.
--> Proposed novel RL formulation allows for gate and wsapw to be performed in the same timestep.



- Cost function
- 


- BRIDGE gate
    > SWAP-only routing algorithmに適切に追加することで性能向上が見込める
    > [Optimization of Quantum Circuit Mapping using Gate Transformation and Commutation](https://arxiv.org/abs/1907.02686)

## Data

## Impact


## What's next?


## Related papers / repo
- [HER 18]: https://arxiv.org/abs/1812.11619 
- 
- [Optimal Layout Synthesis for Quantum Computing](/G4yhNekWQ2y4dFS8Kdp08A)
- https://github.com/Macro206/qubit-routing-with-rl/tree/master/agents

