---
theme: prussianblue
contents:
  - Preliminary
  - Introduction
  - Framework
  - Evaluation
  - Related Work
  - Conclusion
title: IEEE TDSC
---

# IEEE TDSC

<br>

## **Blockchain-Based Transparency Framework for Privacy Preserving Third-Party Services**
<br>
<br>

#### Runhua Xu, Chao Li (Member IEEE) 
#### James Joshi (SeniorMember IEEE)

<div class="pt-12">
  <span> 
    <i>VOL. 20, NO. 3, MAY/JUNE 2023</i>
  </span>
</div>

<!--

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />


<br>
<br>
<br>

# TPA-Based Cryptosystems and Applications

- Fully Trusted
- Challenge
  - incentive mechanisms
  - transparent mechanism
  - honest-but-curious participants

<!-- <img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_32_1_20231016113200.png" class="mx-auto" /> -->
<!-- <img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_31_42_20231016113141.png" class="mx-auto" /> -->
<!-- <img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_36_40_20231016113640.png" class="mx-auto" /> -->
<!-- <img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_17_8_38_20231016170838.png" class="mx-auto" /> -->

<!--
- 在传统的数据统计收集方式中,当查询发送到云服务器时,云服务器直接收集用户数据,计算查询统计信息,并回答查询。在这种场景下,数据收集器或传感器服务器需要被信任.
- 各种数据泄露事件突显了依靠数据收集者(例如Equifax)来保护用户私人数据的困难
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>


# Attribute-Based Encryption (ABE)

<!-- <img src="" class="mx-auto" width="570" /> -->

$$
\mathcal{E}_{ABE}=(Setup, KeyGeneration, Encrypt, Decrypt)
$$


# Functional Encryption (FE)

$$
\mathcal{E}_{FE}=(Setup, KeyDerive, Encrypt, Decrypt)
$$

# Comparing ABE and FE

- ABE: Data user attributes
- FE: Function-related vector

<!--

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# FE-Based Application and Potential Privacy Leakage

<!-- <img src="" class="mx-auto" /> -->

Privacy-preserving machine learning

dp

mpc

<!--
PPML的主要方法包括:
- 加密算法:如功能加密,同态加密等,在加密数据状态下进行计算。
- 安全多方计算协议:多个实体共同计算,但不能获取对方私有数据。
- 差分隐私:在结果中加入噪声保护隐私。
- Federated Learning:分布式协作学习。
通过这些技术手段,PPML可以在多个机构之间开展协作学习,同时保护数据隐私。
这对金融、医疗等领域的数据分析具有重要意义。
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# HE 同态加密

- **Encode: item $v \to$ encoded value $x \in D$**
- **Perturb: randomly perurbs $x \to y$ in $D$**
- **Aggregate: estimate frequency from $y$**



<!--

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# MPC 安全多方计算


<!--

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>


# Authority Transparency

Authority transparency is defined as a publicly auditable set of a TPA’s activities.

- Obligations
- Public parameter distribution $\mathcal{O}_{pp}$
- Trustworthy key service $\mathcal{O}_{ks}$

# Definition

$$
\mathcal{AT}_{\mathcal{O}}^{\mathcal{T},\mathcal{L},\mathcal{C}}=(\mathrm{Gen}_{\mathcal{O}},\mathrm{Log}_{\mathcal{O}_{pp}},\mathrm{Log}_{\mathcal{O}_{ks}},\mathrm{Check}_{\mathcal{O}},\mathrm{Inspect},\mathrm{Gossip})
$$

<!--

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Blockchain

- records
- transactions
- digital events that have been executed and shared 

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Ethereum

- open-source
- public blockchain-based
- distributed computing platform
- support smart contracts
- Tow types of accounts
  - EOAs    
  - Contract Accounts

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Smart Contract
refer to a piece of code  
  - Solidity program code
    - functions    
    - parameters    
    - modifiers
  - Deploy
    - corresponding bytecodes    
    - ABI application binary interface    
  - Send a contract transaction to Ethereum network
  - The miners will include the bytecodes into the newly coming block

---
id: 2
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# General Data Protection Regulation (GDPR)

# California Consumer Privacy Act (CCPA)

# Certificate Authorities (CAs)

# Key Directories (KDs)

---
id: 2
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Challenge

- commercial companies 
- non-profit organizations

---
id: 2
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Contributions

- First
- Next
- Also
- Finally


---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Overview of TAB

- TPA have additional responsibilities
  - submit public parameters Opp
  - reporting its fulfillment in the key service
  - verifying the record

- Actors
  - all users of an crypo-based app
  - data owner: encryption
  - data user: decryption
  - fulfill Oks

- Monitors
   - inspecting the contents of the recorded auditing obligations
   - find suspicious obligations
   - data owner and independent entities play the role of the monitors

- Administrator
   - deployment
   - maintenance
   - administration

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>
<br>

# Notations and Use Scenarios

We use B to represent the Ethereum blockchain, and let BTAB SC denotes our proposed smart contract deployed in the blockchain

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Threat Model

<!-- <img src="/rma.png" class="mx-auto" /> -->

some common assumptions

- a centralized TPA or key server is assumed to be fully trusted and 
- both decryption and encryption entities are assumed to be honest-but-curious.

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Threat Model of Privacy-Enhanced Applications


---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Threat Model of TAB

> Note that misbehavior may be related to non-malicious misuse by normal actors or the behavior of compromised actors controlled by an attacker.

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>
<br>

# Potential Collusion
> Rather than forbidding or preventing collusion through technical means, such collusion between two stakeholders (i.e., TPA and actors) can be solved by resorting to game theory and incentive mechanism designed in the smart contracts.

- Game Theory
- Incentive mechnism in smart contracts

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Public Parameter Audit Obligation (PPAO)

$$
\mathcal{O}_{p p}^{e}:=\mathrm{H}\left(e_{i d}\right):\left\langle e_{i d}, \mathrm{pk}_{e}, \operatorname{Sig}_{\mathrm{sk}_{e}}\left(e_{i d}, \mathrm{pk}_{e}\right)\right\rangle
$$

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Key Service Audit Obligation (KSAO)

$$
\mathcal{O}_{k s}^{\mathcal{C}^{\text {actor }}, \mathcal{A}}:=\mathrm{H}\left(\mathcal{C}_{i d}^{\text {actor }}, \mathcal{A}_{i d}, r\right):\left\langle\mathcal{S}_{\text {req }}, \mathcal{S}_{\text {resp }}\right\rangle
$$

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# TAB Model

$$
\mathcal{M}_{\mathcal{O}}^{\mathcal{A},\mathcal{B},\mathcal{C}}=(\mathrm{Gen}_{\mathcal{O}},\mathrm{Log}_{\mathcal{O}_{pp}},\mathrm{Log}_{\mathcal{O}_{ks}},\mathrm{Inspect})
$$

- $\mathcal{A}$ Authority
- $\mathcal{B}$ Blockchain
- $\mathcal{C}$ Actor
- $\mathcal{C}.actor$ functional module
- $\mathcal{C}.monitor$ monitoring modules


<!-- 
As TAB adopts the Ethereum blockchain as the underlying public ledger infrastructure, 
there is no need to run the gossip and check protocols 
because these logging-related functions are the features provided by the Ethereum smart contract
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Design of $\mathcal{B}_{SC}^{TAB}$

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_31_19_20231016113119.png" class="mx-auto" />

- administrative module
- access control module
- obligation module
- inspection module
- incentive module

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Operation Mechanism

first need to register and pay the cost by themselves.
Besides, we make the TPA and data users make a guaranteed deposit after the registration phase.
If monitors find the malicious behaviors, they will acquire the reward from a fine to the corresponding entity
Without the guaranteed deposit, the corresponding entity is not allowed to operate in/join the system.

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# TAB Procedures

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_30_38_20231016113038.png" class="mx-auto" />

<!-- 
- 但在TAB系统中,TPA不是完全可信任的。- 为了解决这个问题,我们提出了一个不同的方法。- 该方法是在智能合约中部署IPM,而不是在TPA内部。- 智能合约是公开透明的,不受TPA控制。- 这样可以去掉对TPA的信任要求,提高系统的可靠性。- 将IPM放在智能合约中也有利于公平性。总之,我们的方法克服了只在TPA内部部署IPM的缺点,通过在智能合约中部署IPM增强了TAB系统的安全性和公平性。
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Applicability of TAB
TAB is applicable to ABE-based applications by replacing the following audit obligations:

$$
\mathcal{S}_{\mathrm{req}}^{\mathcal{C}_{j}^{\mathrm{user}}}=\langle r^{\prime},\boldsymbol{y}_j,t_{\mathcal{C}_{j}^{\mathrm{user}}},\mathrm{Sig}_{\mathrm{sk}_{\mathcal{C}_{j}^{\mathrm{user}}}}(r^{\prime},\boldsymbol{y}_j,t_{\mathcal{C}_{j}^{\mathrm{user}}})\rangle,
$$

$$
\mathcal{S}_{\mathrm{resp}}^{\mathcal{A}}=\langle r^{\prime},\mathrm{H}(\mathrm{sk}_{\boldsymbol{y}_{j}}^{\mathrm{FE}}),t_{\mathcal{A}},\mathrm{Sig}_{\mathrm{sk}_{\mathcal{A}}}(r^{\prime},\mathrm{H}(\mathrm{sk}_{\boldsymbol{y}_{j}}^{\mathrm{FE}}),t_{\mathcal{A}})\rangle,
$$

by the corresponding audit obligations:

$$
\mathcal{S}_\mathrm{req}^{\mathcal{C}_j^{\mathrm{user}}}=\langle r^{\prime},S_j,t_{\mathcal{C}_j^{\mathrm{user}}},\mathrm{Sig}_{\mathrm{sk}\mathcal{C}_j^{\mathrm{user}}}(r^{\prime},S_j,t_{\mathcal{C}_j^{\mathrm{user}}})\rangle,
$$

$$
\mathcal{S}_{\mathrm{resp}}^{\mathcal{A}}=\langle r^{\prime},\mathrm{H}(\mathrm{sk}_{\mathcal{S}_{j}}^{\mathrm{ABE}}),t_{\mathcal{A}},\mathrm{Sig}_{\mathrm{sk}_{\mathcal{A}}}(r^{\prime},\mathrm{H}(\mathrm{sk}_{\mathcal{S}_{j}}^{\mathrm{FE}}),t_{\mathcal{A}})\rangle,
$$


---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Security Guarantee

- log-consistency
- unforgeable-service
- non-fabrication

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Privacy Guarantee


---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Trustworthiness Goal


---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Experimental Evaluation


---
id: 5
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Privacy Enhanced Applications



---
id: 5
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Transparency


---
id: 5
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Blockchain

---
id: 6 
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Conclusion

<br>

- #### **Key-value LDP protocols are vulnerable to poisoning attacks**

<br>

- #### **An attacker can promote frequency/mean of any target items**

<br>

- #### **We highlight the need for strong defenses against such attacks**

<br>

> *Our defends help to degree, but there is more work to do.*


