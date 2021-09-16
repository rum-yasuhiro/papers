# A Hardware-Aware Heuristic for the Qubit Mapping Problem in the NISQ Era

## Information about
- Authors: 
  > Siyuan Niu, Adrien Susu, Gabriel Staffelbach, Aida Todri-Sanial
- Pub info:
  > IEEE Transactions on Quantum Engineering ( Volume: 1)　<br>
  > 10.1109/TQE.2020.3026544
- Funding:
  > 

## Key Ideas and one paragraph abstraction


提案手法

nisq向けのHardware-awareなコンパイラ（レイアウト、ルーティング）

### ルーティング
- HA SWAP and Bridge based heuristic search
SABRE: SWAPに焦点を当てたheuristic
トポロジーとcalibrationを考慮したdistance matrixを構成し各コストを減らす
SABREと違って、Qubitの移動にSWAPを使うかBridgeを使うか最適化する

DAGに変換

#### Heuristic Cost function (H)
DAGの各ステップごとの可能なSWAPのコストを推定する
距離を考慮して最適なSWAPを選択
SWAPはその先のステップに影響を与えるためlookaheadする必要がある
コストを評価するための行列
- SWAP matrix
  > 行列要素(i, j)は量子ビットiからjまでの最短距離（最小SWAP数）を格納する <br>
  > Floyd-Warshall algorithmで効率的に行列を作る
  > https://dl.acm.org/doi/10.1145/367766.368168
- swap error matrix
  > 行列要素(i, j)は量子ビットiからjまでのエラー率（最小構成SWAP数をcalibrationデータに照合）を格納する
  > swapのエラー率は大きい方をとる
  > Floyd-Warshall algorithmで効率的に行列を作る
- swap execution time atrix
  >  SWAP実行時間が各要素
  >  Floyd-Warshall algorithmで効率的に行列を作る 
これに加え、優先度付けのための各行列に対する重みを定義

- Distance matrix D
> 各行列を重みつきで足し合わせたもの <br>
> $$D=\alpha_{1} \times S+\alpha_{2} \times \mathcal{E}+\alpha_{3} \times T$$

レイアウト
- hardware-aware simulated annealing(HSA)

OpenQASMとデバイスのcalibrationデータを入力とする


## Context

## Data

## Impact
