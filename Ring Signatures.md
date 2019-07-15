# Ring Signatures

---

## Origin Paper

Ring Signatures[^1]

## Ring Signatures ?

* “How to leak a secret” 논문집에 실린 논문 중 하나로 알고리즘 프로세스가 그룹 내에서 돌고 도는 모양이 마치 ring 모양 같다고 하여 Ring signatures로 명명된 그룹 암호화 알고리즘
* Ring signatures에는 미리 정해진 그룹 X, 그룹을 설정/변경/삭제하는 절차 X, 실제 서명자의 익명성을 취소할 방법 X
* Ring signatures를 만들기 위해서 실제 서명자는 자신을 포함한 가능한 구성원의 임의 집합을선언하고 자신의 private key와 다른 구성원들의 public key만을 사용하여 서명을 혼자서 계산해 냄
* 그룹 내에서 메시지에 대해 서명이 필요할 때 그룹 내부에서 각각 구성원의 private key와 public key를 이용해 서명을 하지만 그룹 외부에서 볼 때에는 누구의 key가 사용되어 서명이 되었는지 확인할 수 없음 (뒤에서 “White House” 예를 들어 설명)
* 알고리즘은 Linear한 특징을 지니고 있어 Ο(𝑛)의 시간 및 공간 복잡도를 보임

## History

- CryptoNote Tech.에서 처음으로 Ring signatures를 사용

- 코인 중에서는 Bytecoin에 Ring signatures가 처음으로 적용

- ShadowCash는 Ring signatures를 사용해 트랜잭션의 Sender & Receiver를 익명화 -> 버그가 발견 -> 2016년 2월까지 Receiver만 익명화가 된 트랜잭션 부분 익명화로 수정

- Monero는 Ring signatures를 이용하여 블록체인 상에서 트랜잭션의 내용을 난독화 -> 송금을 하는 사람과 받는 사람만 실제 거래 금액을 알 수 있음

- 이후 Monero는 더 빠르고 진보된 방식인 Bulletproofs로 익명화 방식을 바꿈

## White House Leak Dilemma

![1563176382197](C:\Users\Ing\AppData\Roaming\Typora\typora-user-images\1563176382197.png)

![1563176391993](C:\Users\Ing\AppData\Roaming\Typora\typora-user-images\1563176391993.png)

[1^]: Ring Signatures: Stronger Definitions, and Constructions without Random Oracles. Adam Bender, Jonathan Katz, Ruggero Morselli. Advances in Cryptology - Asiacrypt 2001

