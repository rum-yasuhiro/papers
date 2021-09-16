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
- gateが実行されるtime stepを考慮すると，RLは最適解を判断できない
  > --> SWAP depthを最短にする技術を追加
- near-term architecture sizeにrandom circuitで他を凌駕


## Context

## Technical Terms
- Qubit routing
    > the task of modifying quantum circuits so that they satisfy the connectivity constraints of a target quantum computer.
    > They involves inserting SWAP gate into the circuit so that the logial gates only ever occure between adjacent physical qubits. 
    > The gal is to minimise the circuit depth added by the SWAP gates.

deep Q-learning

- Reinforcement Learning
    > [Reinforcement Learning](/0EJae6qmQ2axwghTgKsLmg)
    - State
        > プロセッサと量子回路の実行具合
        > 
        > N: 物理ノード，
        > Q: 論理量子ビット(logical qubits)
        > Qubit location: N-->Q
        > Qubit targets: Q-->Q
        > Circuit progress Q --> $N_{d+1}$
    - Reword
        > 報酬が出されるタイミング
        > - ゲートがスケジュールされた時
        > - 
    - Action 
        > 並列で実行できるSWAPのセット

- Markov Decision Process(MDP)


- BRIDGE gate
    > SWAP-only routing algorithmの性能を向上させる手法
    > 

## Data

## Impact

## Related papers / repo
- [HER 18]: https://arxiv.org/abs/1812.11619 
- 
- [Optimal Layout Synthesis for Quantum Computing](/G4yhNekWQ2y4dFS8Kdp08A)
- https://github.com/Macro206/qubit-routing-with-rl/tree/master/agents

