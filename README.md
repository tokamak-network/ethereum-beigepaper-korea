# Ethereum_beigepaper_korea
온더(Onther Inc.)에서 번역한 이더리움 베이지 페이퍼입니다.
아직 초안이며, 수정 및 보완검토가 필요합니다. [이슈](https://github.com/Onther-Tech/ethereum-beigepaper-korea/issues)와 [pull request](https://github.com/Onther-Tech/ethereum-beigepaper-korea/pulls)를 통해 더 나은 번역이 될 수 있도록 많은 참여 부탁드립니다.


# PDF 빌드

[markdown-pdf](https://github.com/alanshaw/markdown-pdf)를 사용하여 md파일을 pdf파일로 빌드할 수 있습니다.  

원본: https://github.com/chronaeon/beigepaper/blob/master/beigepaper.pdf

require : `node` 및 `npm` 

```
npm install markdown-pdf
node build-pdf.js
```



# 목차
* [Abstract](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/abstract.md)

1. [Imagining Bitcoin As a Computer](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/1_Imagining_Bitcoin_as_a_Computer.md)
   1. [Native Currency](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/1_Imagining_Bitcoin_as_a_Computer.md#native-currency)
2. [Memory and Storage](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md)
   1. [World State](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#world-state)
      1. [merkle patricia trees](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#merkle-patricia-trees)
   2. [Tree Terminology](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#tree-terminology)
      1. [Recursive Length Prefix Encoding](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#recursive-length-prefix-encoding)
   3. [The Block](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#the-block)
      1. [The Block Header](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#the-block_header)
      2. [Block Footer](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#block-footer)
      3. [Block Number and Difficulty](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#block-number-and-difficulty)
      4. [Account Creation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#account-creation)
      5. [Account State](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#account-state)
      6. [Bloom Filter](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#bloom-filter)
      7. [Transaction Receipts](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage.md#transaction-receipts)
3. [Processing and Computation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#processing-and-computation)
   1. [The Transaction](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#the-transaction)
      1. [Transactions Root](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#transactions-root)
   2. [State Transition Function](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#state-transition-function)
   3. [Mining](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#mining)
   4. [Verification](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#verification)
   5. [Sender Function](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#sender-function)
   6. [Serialization/Deserialization](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#serialization/deserialization)
   7. [Ethereum Virtual Machine](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#ethereum-virtual-machine)
      1. [Fees](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#fees)
   8. [Execution](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#execution)
      1. [Intrinsic Validity](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#intrinsic-validity)
      2. [Transaction Receipt](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#transaction-receipt)
      3. [Code Deposit](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#code-deposit)
      4. [Execution Model](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#execution-model)
      5. [Execution Overview](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#execution-overview)
      6. [The Execution Cycle](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#the-execution-cycle)
      7. [Message Calls](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#message-calls)
      8. [Contract Creation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#contract-creation)
      9. [Execution Environment](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#execution-environment)
      10. [Big Endian Function](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#big-endian-function)
   9. [Gas](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#gas)
      1. [Gas Price/Gas Limit](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#gas-price/gas-limit)
      2. [Machine State](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#machine-state)
      3. [Exceptional Halting](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#exceptional-halting)
      4. [EVM Code](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#evm-code)
   10. [Blocktree to Blockchain](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#blocktree-to-blockchain)
   11. [Ommer Validation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#ommer-validation)
   12. [Transaction Validation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#transaction-validation)
   13. [Reward Application](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#reward-application)
   14. [Mining Proof-of-Work](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#mining-proof-of-work)
       1. [Ethash: Seed->Cache->Dataset->Slice](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#ethash)
       2. [Difficulty Mechanism](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#difficulty-mechanism)
   15. [Pseudorandom Numbers](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#pseudorandom_numbers)
   16. [Chainsize Limits](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#chainsize-limits)
   17. [Scalability](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#scalability)
       1. [Sharding](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#sharding)
       2. [Casper](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#casoer)
       3. [Plasma](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation.md#plasma)
A. [EVM OpcodesButerin2017](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/EVM-OpcodesButerin2017.md)

* [Reference](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/Reference.md)
