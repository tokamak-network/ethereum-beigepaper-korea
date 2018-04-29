# Ethereum_beigepaper_korea
온더(Onther Inc.)에서 번역한 이더리움 베이지 페이퍼입니다.
아직 초안이며, 수정 및 보완검토가 필요합니다. [이슈](https://github.com/Onther-Tech/ethereum-beigepaper-korea/issues)와 [pull request](https://github.com/Onther-Tech/ethereum-beigepaper-korea/pulls)를 통해 더 나은 번역이 될 수 있도록 많은 참여 부탁드립니다.


# PDF 빌드

[markdown-pdf](https://github.com/alanshaw/markdown-pdf)를 사용하여 md파일을 pdf파일로 빌드할 수 있습니다.  

require : `node` 및 `npm` 

```
npm install markdown-pdf
node build-pdf.js
```



# 목차
* [Abstract](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/abstract.md)

1. [Imagining Bitcoin As a Computer](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/1_Imaginig_Bitcoin_As_a_Computer)
   1. [Native Currency](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/1_Imaginig_Bitcoin_As_a_Computer)
2. [Memory and Storage](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
   1. [World State](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      1. [merkle patricia trees](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
   2. [Tree Terminology](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      1. [Recursive Length Prefix Encoding](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
   3. [The Block](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      1. [The Block Header](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      2. [Block Footer](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      3. [Block Number and Difficulty](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      4. [Account Creation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      5. [Account State](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      6. [Bloom Filter](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
      7. [Transaction Receipts](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/2_Memory_and_Storage)
3. [Processing and Computation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   1. [The Transaction](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      1. [Transactions Root](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   2. [State Transition Function](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   3. [Mining](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   4. [Verification](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   5. [Sender Function](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   6. [Serialization/Deserialization](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   7. [Ethereum Virtual Machine](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      1. [Fees](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   8. [Execution](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      1. [Intrinsic Validity](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      2. [Transaction Receipt](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      3. [Code Deposit](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      4. [Execution Model](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      5. [Execution Overview](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      6. [The Execution Cycle](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      7. [Message Calls](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      8. [Contract Creation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      9. [Execution Environment](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      10. [Big Endian Function](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   9. [Gas](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      1. [Gas Price/Gas Limit](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      2. [Machine State](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      3. [Exceptional Halting](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
      4. [EVM Code](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   10. [Blocktree to Blockchain](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   11. [Ommer Validation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   12. [Transaction Validation](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   13. [Reward Application](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   14. [Mining Proof-of-Work](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
       1. [Ethash: Seed->Cache->Dataset->Slice](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
       2. [Difficulty Mechanism](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   15. [Pseudorandom Numbers](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   16. [Chainsize Limits](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
   17. [Scalability](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
       1. [Sharding](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
       2. [Casper](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
       3. [Plasma](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/3_Processing_and_Computation)
A. [EVM OpcodesButerin2017](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/)

* [Reference](https://github.com/Onther-Tech/ethereum-beigepaper-korea/blob/master/Reference)
