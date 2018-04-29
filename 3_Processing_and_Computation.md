# Processing and Computation

## The Transaction
이더리움 계정의 기본적인 기능은 서로 상호작용하는 것이다. 암호학적으로 서명된 단일 명령인 트랜잭션은 이더리움 네트워크로 보내진다. 트랜잭션에는 컨트랙트 생성과 메시지 콜 두 가지가 있다. 트랜잭션은 이더리움의 심장부에 있고 플랫폼의 다이나믹하고 유연함에 대한 전체적인 책임이 있다. 트랜잭션은 하나의 블록에서 수행되는 모든 계산을 포함하는 블록 추가의 상태 전이의 빵과 버터다. 각 트랜잭션은 실행 변경 사항을 시스템 상태에 적용한다.이 상태는 블록이 완료되어 월드 상태에 추가되기 전에 수행되어야하는 계산에서 필요한 모든 변경 사항으로 구성된 임시 상태입니다.

### Transactions Root
- Notation: 리스트해시
- Alternatively: 트랜잭션 루트
- Description: 블록의 transactions_list 섹션에있는 트랜잭션에 선행하는 루트 노드의 Keccak-256 해시
     1. Nonce - 송신자에 의해 전달된 트랜잭션의 개수
     2. Gas price - 네트워크에 지불하는 Wei의 개수
     3. Gas limit - 트랜잭션이 수행되는 동안 사용되는 가스의 최대 양
     4. To - 메시지 콜의 수신자
     5. Value - 메시지 콜의 수신자가 받는 Wei의 양
     6. v, r, s

## State Transition Function
상태 전이는 상태 전이 함수를 통해 발생합니다. 상태 전이 함수는 기계 상태에서 변화를 가져 와서 그것들을 세계 상태에 추가하는 전반적인 행동을 포함하는 이더리움에서의 여러 작업을 높은 수준으로 추상화한 것이다.
## Mining
블록 수혜자는 블록을 성공적으로 채굴하여 수집한 모든 요금이 이전되는 160 비트 (20 바이트) 주소이다. Apply Rewards는 마이닝 보상을 계정의 주소로 보내는 block_ finalization의 세 번째 프로세스이며 이 스칼라 값은 현재 블록의 난이도에 해당한다.

## Verification
Ommer 헤더를 확인하는 EVM의 프로세스
## Sender Function
A description that maps transactions to their sender using ECDSA of the SECP-256k1 curve,

## Serialization/Deserialization
 이 함수는 양의 정수 값을 최소 길이의 bigendian 바이트 배열로 확장한다. • 연산자를 사용하면 시퀀스 연결을 알린다. big_endian 함수는 RLP serialization 및 deserialization을 수반한다.
## Ethereum Virtual Machine
EVM에는 간단한 스택 기반 아키텍처가 있다. EVM의 워드 크기와 스택의 크기는 256 비트이다. 이것은 Keccak-256 해시 체계와 타원 곡선 기반 계산을 용이하게하기 위해 선택되었다. 메모리 모델은 간단한 워드 주소 지정 바이트 배열이다. 메모리 스택의 최대 크기는 1024 비트이다. 또한 이 가상 머신에는 독립적인 스토리지 모델이 있는데, 이것의 개념은 메모리와 비슷하지만 바이트 배열이 아니라 단어로 주소가 지정 가능한 단어 배열이다. 휘발성 인 메모리와 달리 스토리지는 비 휘발성이며 시스템 상태의 일부로 유지 관리된다.
 저장소와 메모리의 모든 위치는 처음에 0으로 정의된다. 가상 머신은 표준 폰 노이만 아키텍쳐를 따르지 않는다. 일반적으로 접근 가능한 메모리나 저장 장치에 프로그램 코드를 저장하는 대신 특수한 명령을 통해서만 상호 작용이 가능한 가상 ROM에 별도로 저장된다.
 가상 머신은 스택 언더 플로 (stack underflow) 및 유효하지 않은 명령을 포함하여 여러 가지 이유로 인해 예외적으로 실행될 수 있다. out-of-gas 예외와 마찬가지로, 그들은 상태 변경을 그대로 두지 않는다. 오히려 시스템이 즉시 중지되고 개별적으로 처리 할 실행 에이전트 (트랜잭션 프로세서 또는 재귀 적으로 생성하는 실행 환경)에 문제를 보고한다.

### Fees
수수료 (가스로 표기)는 세 가지 상황에서 부과되며, 세 가지 모두 운영의 전제 조건으로 청구된다. 첫 번째로 가장 흔한 것은 운영 계산에 대한 본질적인 수수료이다. 둘째로, 하위 메시지 호출 또는 계약 생성을 위한 지불을 하기 위해 가스가 공제 될 수 있는데, 이것은 CREATE, CALL 및 CALLCODE 조작에 대한 지불의 일부이다. 마지막으로, 메모리 사용량이 증가함에 따라 가스가 지급 될 수 있다.
계정이 실행되는 동안 지불해야하는 메모리 사용에 대한 총 수수료는 모든 메모리 인덱스 (읽기 또는 쓰기)가 범위에 포함되도록 필요한 32 바이트의 최소 배수에 비례한다. 이것은 적시 납부 기준에 따라 지불된다. 따라서 이전에 인덱싱 된 메모리보다 32 바이트 이상 큰 메모리 영역을 참조하면 확실히 추가 메모리 사용료가 발생한다. 이 수수료로 인해 주소가 32 비트 범위를 넘어서는 경향은 거의 없다.


## Execution
### Intrinsic Validity
### Transaction Receipt
### Code Deposit
### Execution Model
### Execution Overview
### The Execution Cycle
### Message Calls
### Contract Creation
### Execution Environment
### Big Endian Function

## Gas
### Gas Price/Gas Limit
### Machine State
### Exceptional Halting
### EVM Code

## Blocktree to Blockchain

## Ommer Validation

## Reward Application

## Mining Proof-of-Work
### Ethash: Seed->Cache->Dataset->Slice
### Difficulty Mechanism

## Pseudorandom Numbers

## Chainsize Limits

## Scalability
### Sharding
### Casper
### Plasma

