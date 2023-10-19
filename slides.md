---
theme: prussianblue
contents:
  - Preliminary
  - Introduction
  - Framework
  - Evaluation
  - Conclusion
title: IEEE TDSC
---

# IEEE TDSC

<br>

#### **Blockchain-Based Transparency Framework for Privacy Preserving <br>Third-Party Services**
<br>
<br>

#### **Runhua Xu, Chao Li** *(Member IEEE)*
#### **James Joshi** *(SeniorMember IEEE)*

<div class="pt-12">
  <span> 
    <i>VOL. 20, NO. 3, MAY/JUNE 2023</i>
  </span>
</div>

<!--
基于区块链的透明框架:实现第三方服务的隐私保护
- 提出了一个TAB框架,
- 利用区块链技术使第三方机构和设施变得透明可信,
- 服务于加密型的隐私保护应用。
本文提出了TAB框架,使用区块链技术为新兴的基于加密的隐私保护应用提供第三方机构和第三方设施的透明性和可信赖性。主要内容包括:
1. 信息系统日益依赖第三方设施(如云服务、边缘节点),导致日益严重的网络安全和隐私问题。
2. 安全相关的服务和基础设施(如证书机构、第三方密钥管理机构)对建立加密应用的信任至关重要。
3. 提出TAB框架,使用区块链技术使第三方机构透明可审计,保障其可信赖性。
4. TAB使用以太坊区块链作为公共账本,并设计了智能合约以实现问责机制。
5. 提出激励机制鼓励用户参与审计,并惩罚恶意行为。
6. 实验评估了TAB的效率,证明了其安全性,并分析了其提供的隐私保护和可信度。
总之,本文设计了TAB框架,基于区块链实现第三方服务的透明度和可信度,为加密privacy应用建立信任基础。
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />


<br>
<br>
<br>

# TPA-Based Cryptosystems and Applications

<br>

<mimage layout="r" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_10_32_17_tpa.png" class="right-10 absolute" width="400" />

**Assumptions**
  > - ***Fully Trusted***
  > - ***Honest-But-Curious***

**Challenge**
  > - ***Incentive Mechanisms***
  > - ***Transparent Mechanism***
  > - ***Honest-But-Curious Participants***


<!--
1. 新兴的现代加密方案正在被广泛采用。
2. 特别是依赖第三方机构(TPA)提供密钥服务的方案。
3. 这些方案被隐私保护应用所采用。
4. 在这些应用中,数据被加密。
5. 数据管理操作(查询、访问控制、计算等)在加密的数据上进行。
6. 这样可以实现在保护隐私的同时进行数据操作。
7. 第三方机构在提供可信可靠的密钥服务方面起关键作用。

- 激励机制(incentive mechanisms):通过给予一定激励来鼓励特定行为。
- 参与者(participant):这里指可能担任机构角色的第三方实体。
- 机构(authority):这里指需要担任某规则角色的一方。
- 意思是使用激励措施鼓励第三方实体自愿地担任机构的角色和责任。
- 这样可以避免单一中心化的机构,实现多方共同监管。
- 透明指的是通过主动公开披露相关信息,而不是隐藏或保密,以便外部可以监测和验证,保证系统的可信度
- 诚实即为参与者不会伪造数据，服务器也不会对参与者上传的数据进行攻击、破译或逆向工程等恶意操作。　　
好奇是，服务器方对用户的原始数据有一定程度的好奇，并且可能会绕过一些安全措施直接访问用户的原始数据。　另外，在联邦学习环境下，服务器因为能够获得多方上传的更新梯度，所以能够获得他人的数据。成员之间不会互相传递数据，但可以串通。多个成员串通可以大规模的伪造数据，从而导致最终模型的失败或被恶意方控制。

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Attribute-Based Encryption (ABE)


$$
\pmb{\mathcal{E}_{ABE}=(Setup, KeyGeneration, Encrypt, Decrypt)}
$$


# Functional Encryption (FE)

$$
\pmb{\mathcal{E}_{FE}=(Setup, KeyDerive, Encrypt, Decrypt)}
$$

<table>
  <td>
    <mimage layout="c" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_11_43_22_abe.png" width="300" />
  </td>
  <td>
    <mimage layout="c" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_11_43_38_fe.png" width="349" />
  </td>
</table>



<!-- 
1. ABE 是一种公钥加密的变体。
2. 在 ABE 中,密文依赖于访问策略,该访问策略定义在一组属性证书(attribute credentials)之上。
3. 属性证书可以是像年龄、隶属组织等属性。
4. 只有持有访问策略指定的合适属性证书的实体,才能获得用于访问加密数据的密钥。
5. 也就是说,加密的数据只有符合访问策略要求的用户才能解密。
6. 这种基于属性和访问策略的方法,使得 ABE 可以实现对加密数据的细粒度访问控制。
综上所述,ABE 通过将密文绑定访问策略与属性证书,实现了身份场景下对加密数据更精细化的访问控制。这是区别于传统公钥加密的一个重要特点。

- FE是在公钥加密基础上推广的一种加密形式。
- 在FE中,可以为用户 issuing 函数密钥。
- 这个函数密钥允许用户计算密文加密内容的某个函数。
- 而不是像公钥加密那样直接解密出原文。
- 举例来说,可以 issuing 一个"年龄大于18"的函数密钥。
- 用户可以用这个密钥来判断密文中的年龄信息是否大于18。
- 但不能解密出具体的年龄数值。
这样FE可以实现对加密数据的函数计算,同时保护隐私。扩展了公钥加密的应用范围。

-->


---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Different Key Service Audit Obligations in FE and ABE

$$
\begin{array}{ccc}\hline\text{Types}&\text{obligations in FE}&\text{obligations in ABE}\\\hline\text{Setup-Output}&\text{private key}&\text{public parameter}\\\text{KeyGen-Input}&\text{function-related vector}&\text{attribute set}\\\text{KeyGen-}&\text{functional decryption}&\text{attribute private}\\\text{Output}&\text{key}&\text{key}\\\hline\end{array}
$$

<br>

# Encryption Scheme

|         | **Setup** | **Key Derive/Generation** | **Encrypt**  | **Decrypt** |
| :-----: | :-------: | :-----------------------: | :----------: | :---------: |
| **ABE** |   `TPA`   |           `TPA`           | `Data Owner` | `Data User` |
| **FE**  |   `TPA`   |           `TPA`          | `Data Owner` | `Data User` |

<!--
ABE和FE的主要区别在于生成或派生私钥所使用的证书不同。
具体来说:
1. 在ABE中,私钥是根据用户的属性证书生成的。只有具备访问策略指定属性的用户能生成私钥。
2. 而在FE中,私钥是根据允许的函数类型派生的。用户只能计算特定函数,而不能直接解密。
3. ABE的访问控制是基于属性的。符合属性要求的用户才能解密数据。
4. FE的访问控制是基于函数的。用户只能计算特定函数,不能完全解密。
5. ABE更直接对应访问控制场景。FE提供了更好的保密性。
6. 两者都依赖于第三方机构发放密钥。
- 综上所述,ABE和FE主要区别在于私钥的生成依据不同,前者基于属性,后者基于函数,适用于略有不同的应用场景。
- 但两者都提供了比传统加密更细粒度的访问控制。

属性加密(ABE)的基本流程:
1. 和函数加密类似,Setup和KeyGeneration算法由一个被完全信任的第三方机构(TPA)运行。
2. 数据拥有者使用Encrypt算法和指定的访问策略来保护数据。
3. 数据用户持有满足访问策略的正确属性证书,可以使用Decrypt算法访问(解密)加密的数据。
4. 也就是说,只有属性证书满足访问策略要求的用户,才能够解密数据。
5. 访问策略中的属性要求控制着哪些用户可以访问数据。
6. 这样ABE实现了对加密数据的细粒度访问控制。
7. 第三方机构负责发放用户的属性证书。
综上,ABE通过访问策略和属性控制来保护数据,并只允许授权用户访问。
FE:
1. Setup 和 KeyDerive 算法由一个被完全信任的第三方机构(TPA)运行。
2. 数据拥有者可以使用 Encrypt 算法来保护其数据。
3. 数据用户持有由其第三方机构颁发的函数解密密钥,可以使用 Decrypt 算法在密文上计算函数,得到函数结果。
4. 在这个过程中,数据用户无法学习到原始数据。
5. 也就是说,函数加密允许数据用户对加密数据进行函数计算,而不能直接获知原始数据。
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# FE-Based Application

- **Privacy-Preserving Machine Learning**

> - ***Functional encryption***<br>
> - ***Homomorphic encryption***<br>
> - ***Secure Multiparty Computing Protocol***

- **Federated Learning Learning**

> - ***Differential Privacy***<br>

<br>

# Potential Privacy Leakage

> ***The third party is honest but curious***

> ***Exploit a manipulated vector***

<!--
PPML的主要方法包括:
- 加密算法:如功能加密,同态加密等,在加密数据状态下进行计算。
- 安全多方计算协议:多个实体共同计算,但不能获取对方私有数据。
- 差分隐私:在结果中加入噪声保护隐私。
Federated Learning:分布式协作学习:
通过这些技术手段,PPML可以在多个机构之间开展协作学习,同时保护数据隐私。
这对金融、医疗等领域的数据分析具有重要意义。
潜在风险：
1. 在PPML方法中,虽然使用了FE方案,但仍存在隐私泄露的潜在风险。
2. 因为即使是经过授权的诚实但好奇的解密方,也可能通过操作解密的输入向量,反复执行解密算法,收集算法的中间数据。
3. 通过分析这些中间数据,可以推断出部分加密数据的信息。
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Homomorphic Encryption

<mimage layout="r" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_12_18_47_he.png" class="right-10 absolute" width="450" />

- **没有碰撞**

> 加密后的两个值相等

> 加密前两个值也是相等的

- **隐藏的性质**

> 加密后这个函数值很难反推出原始的输入值<br>只能用蛮力一个个的去试

- **同态运算**

> - 同态加法

> - 同态乘法

<!--
第一个实现全同态加密算法的科学家：Craig Gentry，也就是数据可用不可见 ，我允许你使用我的数据，但这个数据具体是什么，不能告诉你
核心思想是利用设计的加密函数，能够保证先对这个数据，进行运算然后再加密，跟先对这个数据加密之后再运算是等价的
# 同态加密的性质

- 没有碰撞，与哈希函数不同，应用：加密后的两个值相等==>加密前两个值也是相等的
- 隐藏的性质 hiding property，加密后这个函数值很难反推出原始的输入值，只能用蛮力一个个的去试
- 同态运算，最重要的性质，
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Secure Multi-Party Computing


<mimage layout="r" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_12_8_51_mpc.png" class="right-10 absolute" width="400" />

$\pmb{f(X_1,X_2,X_3,\ldots\ldots,X_n)=(Y_1,Y_2,Y_3,\ldots\ldots,Y_n)}$

- **姚氏百万富翁问题**

- 混淆电路

- 秘密分享

- 不经意传输

# 分类

- 通用

- 特定问题

<!--

-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Authority Transparency

> Authority transparency is defined as a publicly auditable set of a TPA’s activities.

- **Obligations $\pmb{(\mathcal{O})}$**

- **Public Parameter Distribution $\pmb{(\mathcal{O}_{pp})}$**

- **Trustworthy Key Service $\pmb{(\mathcal{O}_{ks})}$**

# Definition

$$
\pmb{\mathcal{AT}_{\mathcal{O}}^{\mathcal{T},\mathcal{L},\mathcal{C}}=(\mathrm{Gen}_{\mathcal{O}},\mathrm{Log}_{\mathcal{O}_{pp}},\mathrm{Log}_{\mathcal{O}_{ks}},\mathrm{Check}_{\mathcal{O}},\mathrm{Inspect},\mathrm{Gossip})}
$$

|    **$\mathcal{T}$**    | **$\mathcal{L}$** | **$\mathcal{C}$** |
| :---------------------: | :---------------: | :---------------: |
| `third-party authority` |   `log server`    |     `client`      |

<!--
1. Authority transparency 指的是第三方机构(TPA)的活动透明性。
2. TPA 是受信任的第三方机构,通常负责关键操作,如发放密钥等。
3. 为了监督TPA,需要公开审计TPA的所有活动。
4. 这些活动构成了一个公开的集合,任何人都可以审查。
5. 这样就实现了对TPA活动的透明审计,这称为 authority transparency。
6. 保证了TPA作为可信方的活动是可验证和可审计的。
总结为:
Authority transparency 是指第三方机构的活动具有公开审计性的的属性。它通过将TPA的活动公开为一个集合来实现对其的监督。

- GenO 是 T 和 C:actor 之间的协议，用于生成要记录的审计义务
- LogOpp 是 T 和 L 之间的协议，用于在公共日志中记录 Opp；
- LogOks 是一个涉及 T、L 和 C:actor 的协议，用于在公共日志中记录 Oks；
- CheckO 是一个涉及 L、C.actor 和 C.auditor 的协议，用于检查日志中是否有审计义务 Opp 或 Oksis
- Inspect 是 L 与 C.monitor 之间的协议，用于允许监控器检查日志内容并查找可疑的审计义务 Oi
- Gossip 是 C.auditor 和 C.monitor 之间的协议，用于比较不同版本的日志，并检测因参与者或代表日志服务器的不当行为造成的任何不一致。
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Blockchain

> A blockchain is a growing list of records (a.k.a, blocks) that are linked via cryptographic techniques, where each block contains a cryptographic hash of the previous block, a timestamp, and the transaction data.

<mimage layout="c" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_13_55_4_Blockchain.jpg" class="right-10 absolute" width="400" />

<br>

- **Records**

- **Transactions**

- **Digital Events**

  > ***that have been executed and shared***

<!-- 
Blockchain是一个不断增长的记录(区块)链条,每个区块通过加密技术与前一个区块连接,并包含以下信息:- 前一个区块的加密哈希值
- 时间戳 
- 交易数据也就是说,blockchain是一串用加密手段连接在一起的区块/记录,新区块中都包含对前一个区块数据的加密证明。这使得blockchain具有不可篡改的特性。
具体而言，区块链是一个公共的分布式数据库，包含已执行并在不同参与者之间共享的记录、交易或数字事件。
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Ethereum

<mimage layout="c" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_14_3_2_ether.png" class="right-10 absolute" width="170" />

- **Open-Source**

- **Public Blockchain-Based**

- **Distributed Computing Platform**

- **Support Smart Contracts**

- **Tow Types of Accounts**

  > - ***External Owned Accounts (EOAs)***

  > - ***Contract Accounts***

<!-- 
1. 以太坊是开源的(open-source)
2. 基于公共区块链(public blockchain-based)
3. 是一个分布式计算平台(distributed computing platform)
4. 支持智能合约(supporting smart contracts)
简言之,以太坊是一个开源的公链平台,可以通过智能合约实现分布式计算。

- 外部拥有账户是与用户相关联的私钥所控制的账户
- 合约账户是分配给智能合约的账户
-->

---
id: 1
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Solidity Program

| <kbd>**functions**</kbd> | <kbd>**parameters**</kbd> | <kbd>**modifiers**</kbd> |
| :---------: |  :---------: |  :--------: |

<br>
<br>

# Smart Contract Deploy

| <kbd>**bytecodes**</kbd> | <kbd>**application binary interface**</kbd> |
| :---------: |  :---------: |  

> - ***Refer to a piece of code***<br>
> - ***Send a contract transaction to Ethereum network***<br>
> - ***The miners will include the bytecodes into the newly coming block***

 

<!-- 
智能合约
- 用户可以编译智能合约生成字节码和ABI
- 然后发送交易,包含字节码和ABI,来部署合约
部署合约的关键步骤是编译生成字节码和ABI,然后通过交易带上它们在以太坊上创建合约。
- 矿工会将字节码打包进新的区块中。
- 每个成功部署的合约账户可以看作是一个小的去中心化计算和存储单元,可以执行合约定义的特定函数,并存储合约允许的数据。
- 函数的输出是确定性的,因为分布式矿工可以确保这一点。
- 在以太坊中,无论是部署智能合约还是调用现有合约的函数都不是免费的。
总结为:
以太坊智能合约通过矿工打包运行,可以实现去中心化的计算和存储。它确定性执行,但需要付费部署和调用
-->

---
id: 2
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Regulations

- **GDPR**

> ***General Data Protection Regulation***

- **CCPA**

> ***California Consumer Privacy Act***

<table>
  <td>
    <mimage layout="c" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_14_50_56_gdpr.jpg" width="180" />
  </td>
  <td>
    <mimage layout="c" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/18_14_51_17_ccpa.jpg" width="180" />
  </td>
</table>

<br>

<!-- 
1. 信息系统正在越来越多地建立在第三方设施或者使用外部服务之上。
2. 对许多企业来说,这降低了成本,让他们可以更专注于核心业务。
3. 另一方面,网络安全事件频发,如数据泄露和身份盗窃,这加剧了用户对自己敏感个人数据的担忧,这些数据存储和处理在第三方平台上。
4. 此外,GDPR和CCPA等法规带来了更严格的合规要求。
5. 企业信息系统需要面对外包带来的安全风险,以及日益复杂的合规性要求。
-->

---
id: 2
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Architectures

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_32_1_20231016113200.png" class="mx-auto" />

<!-- 
一个典型的保护隐私的第三方服务启用系统的体系结构 
一个加密系统模型:
1. 个人数据被加密保护,使用了加密系统。
2. 加密后的数据被第三方IaaS服务收集和处理。
3. 公钥和私钥服务由第三方机构(TPA)提供。
4. 个人数据经过加密,公私钥由TPA管理,加密数据处理由IaaS完成。
5. 这种模型中,数据由加密技术保护,TPA控制密钥,IaaS负责计算,三方分工合作。
6. 个人数据加密由用户自己完成,TPA和IaaS无法访问明文数据。
总结为:
该模型使用加密技术保护个人数据,公私钥管理和计算处理分别由第三方机构和IaaS服务提供,实现职责分离。个人数据经过加密传到IaaS,TPA控制密钥,提高了数据隐私性。
-->
---
id: 2
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Limitations

> - ***Rely on the ABE Cryptosystems***

> - ***Based on a Secure Logging System***

<br>

# Challenges

> - ***Commercial Companies***

> - ***Non-Profit Organizations***

> - ***Concrete Mechanism***

<!-- 
linitation:
简而言之，现有的权威透明提案并不直接支持其他新兴的密码系统，例如已经用于构建安全计算协议的FE和多密钥HE族
challenge:
1. 需要依赖少数大公司来运营安全日志系统,中小机构无法承担。
2. 没有成熟的机制让外部实体进行监督和审计。
3. 因此这种方案想被广泛接受还面临挑战。
4. 需要更易实现和去中心化的方案,降低部署门槛,并让更多实体可参与监督。
5. 还缺乏具体的奖惩机制，让各实体参与透明度框架，监测和审计无意或恶意行为。
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Overview of TAB

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_31_42_20231016113141.png" class="mx-auto" />

<!-- 
展示了 TAB 框架的架构。
- 虚线表示基于加密的隐私保护应用程序的程序，
- 实线表示 TAB 框架的程序。
TAB 由以下实体组成：
- TPA
- Actors
- Monitors
- Administrator
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Entities in TAB

# TPA
> ***The TPA is the same role as in the ordinary FE cryptosystem, but in TAB it has additional responsibilities to fulfill***

- **Submit public parameters**
> ***identity-to-public-key bindings***

- **Verifying the records**
> ***Verifying that the submitted/reported obligations are permanently recorded in the blockchain***

<!--  
TPA 与普通 FE 密码系统中的角色相同，但在 TAB 中，它需要履行额外的职责，包括：
- 提交公共参数义务（特别是身份与公钥绑定），
- 在密钥服务流程中报告其义务履行情况，以及
- 验证提交/报告的义务是否永久记录在区块链中。
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Entities in TAB

# Actors
> ***Actors include all users of an crypto-based privacy-preserving applications***

- **Data owner**
> ***Employ the encryption algorithm***

- **Data user**
> ***Perform secure computation or access control via the decryption algorithm***

- **Fulfill the Obligations**
> ***They are involved in interaction with other actors and/or the TPA***

<!--  
加密隐私保护应用的参与方包括:
1. 使用加密算法的实体(如数据拥有者)
2. 通过解密算法执行安全计算或访问控制的实体(如数据用户)
3. 可能还需承担密钥服务职责的参与方,因为他们需要与其他参与方或第三方机构(TPA)互动
总结:
加密隐私保护应用的参与方包括加密和解密算法的使用者,以及可能需要承担密钥服务职责的互动方。他们既包括数据拥有者,也包括需要访问或计算数据的用户。所有参与密钥分发、加密、解密、访问控制等互动的实体都可以视为参与方
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Entities in TAB

<br>

# Monitors

- **Inspecting the contents**
> ***Monitors are responsible for inspecting the contents of the recorded auditing obligations***

- **Find suspicious obligations**

- **Participating entities**
> ***In TAB, the encryption entities or the additional independent entities play the role of the monitors.***


<!--  
- Monitors负责检查记录的审计义务,找出可疑义务
- 在TAB中,Monitors可以是加密实体(也就是data owner)或独立实体
监控方在透明审计中的责任:
1. 监控方负责检查记录的审计义务的内容,发现可疑的义务。
2. 在透明权威审计(TAB)中,加密实体或额外的独立实体可以担任监控方的角色。
3. 监控方需要审查审计日志,标记出可疑的操作。
4. 作为独立的第三方,监控方可以更客观公正地执行审计。
总结:
监控方在透明审计中负责检查记录的内容找出可疑义务,在透明权威审计中,这个角色可以由加密实体或独立第三方充当。 
-->
---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Entities in TAB

<br>

# Administrator
> An administrator is responsible for the deployment, maintenance, and administration of the smart contract.

<br>

- **Deployment**

- **Maintenance**

- **Administration**

<!--  
管理员在智能合约中的角色和职责:
1. 管理员负责智能合约的部署、维护和管理。
2. 智能合约主要包含三个模块:
(a) 义务记录模块,为实体提供各种交互功能来实现记录、审计和检查与义务相关的要求。
(b) 激励机制,为参与者提供支付和奖励功能。
(c) 推理预防模块,之前在第三方机构中部署。
3. 以太坊区块链可以确保智能合约的可信赖性,也可以确保记录的义务是分布式、开放和防篡改的。
4. 一旦智能合约被部署,就不需要中心化的管理。
总结:
管理员负责智能合约的部署和维护,合约包含义务记录、激励和推理预防模块。以太坊区块链确保分布式、不可篡改的义务记录,无需中心化管理
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Threat Model

<br>

#### ***Threat Model of Privacy-Enhanced Applications***

- **An adversary who attempts to compromise the encrypted data** 

- **A curious entity that launches potential privacy attacks**

<br>

#### ***Threat Model of TAB***
- **A dishonest TPA may attempt to forge a key service proof-of-work without actually providing a valid key service**

- **A dishonest actor may try to incorrectly blame other entities for misbehavior**

<!--  
常见假设:
1. 假设中心化的第三方机构(TPA)或密钥服务器是完全可信的。
2. 假设解密实体和加密实体都是诚实但好奇的。
这意味着:
- 集中式的TPA或密钥服务器不会做任何恶意行为,完全可靠。
- 解密和加密的参与方会遵守协议,但出于好奇可能会试图获取额外信息。
这些通常作为加密系统安全模型的基本假设,即信任中心化节点,对终端用户做较弱的安全假设。这可以简化安全分析和证明,但也限制了模型的适用场景。在更严格的威胁模型下,需要处理中心化节点不可信以及完全恶意用户的情况。

PE APP 威胁模型通常关注两个方面:
- 试图破解加密的对抗方。
- 遵守规则但执行隐私推断的好奇实体。
这类模型假设对抗方会攻击加密数据获取明文,或利用规则中的漏洞推断私人信息。

TAB:
总结:
通常的不诚实对抗方包括TPA和参与方。
- TPA可能伪造工作证明,
- 参与方可能错误指责他人。
- 不当行为可能来自正常用户的误用 
- 或者来自被攻击者控制的参与者。
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Potential Collusion
> ***We note that the case of potential collusion between a dishonest TPA and honest-but-curious actors is not fully considered in this paper***

- **Resort to Game Theory**
> - ***Prisoner's dilemma***
> - ***Rock-paper-scissors***


- **Smart Contracts**
> - ***Automatic Execution*** 
> - ***Immutability***
> - ***Distributed Data Storage***

<!--  
- 与其通过技术手段禁止或防止串通，不如借助博弈论和智能合约中设计的激励机制[29]来解决两个利益相关者（即 TPA 和行为者）之间的串通问题。

# 博弈论
- prisoner's dilemma(囚徒困境)描述了两个囚犯面临承认或不承认罪行的选择,展示了非合作博弈中参与者可能作出非最优选择的情况。
- rock-paper-scissors(石头剪刀布)是常见的匹配 pennies game 模型,两个玩家同时出石头、剪刀或布,获胜规则为石头克剪刀,剪刀克布,布克石头。这展示了零和博弈中的策略选择。
- 这两个模型一个展示非合作博弈,一个展示零和博弈,都能很好地说明博弈论中策略性思考和均衡分析的重要性。

# 智能合约
- Automatic Execution 智能合约的条款定义了各方的权利和义务,代码自动执行这些条款,无需第三方干预
- Immutability 智能合约基于区块链,合同代码和执行情况都是透明的,不可篡改。
- Distributed Data 智能合约数据存储在分布式账本,预防单点故障。

-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Public Parameter Audit Obligation

$$
\pmb{\mathcal{O}_{p p}^{e}:=\mathrm{H}\left(e_{i d}\right):\left\langle e_{i d}, \mathrm{pk}_{e}, \operatorname{Sig}_{\mathrm{sk}_{e}}\left(e_{i d}, \mathrm{pk}_{e}\right)\right\rangle}
$$

<br>

# Key Service Audit Obligation

$$
\pmb{\mathcal{O}_{k s}^{\mathcal{C}^{\text {actor }}, \mathcal{A}}:=\mathrm{H}\left(\mathcal{C}_{i d}^{\text {actor }}, \mathcal{A}_{i d}, r\right):\left\langle\mathcal{S}_{\text {req }}, \mathcal{S}_{\text {resp }}\right\rangle}
$$

<br>

***where each snapshot is a 4-tuple as follows:***

$$
\pmb{\mathcal{S}_{\mathrm{req}}:=\mathrm{H}(\mathcal{C}_{id}^{\mathrm{actor}},\mathcal{A}_{id},r):\langle r,\underline{f},\overline{t}_{\mathcal{C}^{\mathrm{actor}}},\mathrm{Sig}_{\mathrm{sk}_{\mathrm{actor}}}(r,\boldsymbol{f}),t_{\mathcal{C}^{\mathrm{actor}}})\rangle,}
$$

$$
\pmb{\mathcal{S}_{\mathrm{resp}}:=\mathrm{H}(\mathcal{C}_{id}^{\mathrm{actor}},\mathcal{A}_{id},r):\langle r,\boldsymbol{\sigma},t_{\mathcal{A}},\mathrm{Sig}_{\mathrm{sk}_{\mathrm{TPA}}}(r,\sigma,t_{\mathcal{A}})\rangle}
$$

<!-- 
PPAO: 是一个映射结构
- Opp是身份与公钥的绑定，带有签发人的签名
- e_id 表示 e 的描述性标识符，
- H(.) 是哈希函数，
- pk_e 表示实体 e 的公钥绑定，
- Sigsk_e 是使用 sk_e 的签名

KSAO: 是由一对密钥服务快照组成的映射结构
- OC,Aks 是密钥服务的证明。
- 其中r是由密钥服务请求者选择的随机数
- t是每个实体处理的密钥服务的时间戳
- f表示请求内容，例如功能相关向量
- sigma表示TPA已发布密钥的工作量证明
- 
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# TAB Model

<br>

$$
\pmb{\mathcal{M}_{\mathcal{O}}^{\mathcal{A},\mathcal{B},\mathcal{C}}=(\mathrm{Gen}_{\mathcal{O}},\mathrm{Log}_{\mathcal{O}_{pp}},\mathrm{Log}_{\mathcal{O}_{ks}},\mathrm{Inspect})}
$$

|  **$\mathcal{A}$** | **$\mathcal{B}$** | **$\mathcal{C}$** |
| :----------------: | :---------------: | :---------------: |
|   **Authority**    |   **Blockchain**  |     **Actor**     |

<br>
<br>

#### **Theorem**
<br>

> ***If the hash function is collision-resistant and the signature scheme is unforgeable, then TAB model comprises a secure transparency framework.***


<!-- 
- 由于TAB采用以太坊区块链作为底层公共账本基础设施，
- 因此不需要运行gossip和check协议，
- 因为这些与日志相关的功能是以太坊智能合约提供的功能。

如果哈希函数是抗碰撞的，签名方案是不可伪造的，那么TAB模型就构成了一个安全的透明框架。
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Design of $\pmb{\mathcal{B}_{SC}^{TAB}}$
> We use $\mathcal{B}$ to represent the Ethereum blockchain, and let $\mathcal{B}_{SC}^{TAB}$ denotes our proposed smart contract deployed in the blockchain

<mimage layout="r" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_31_19_20231016113119.png" class="right-10 absolute" width="400" />

- **Administrative Module**

- **Access control Module**

- **Obligation Module**

- **Inspection Module**

- **Incentive Module**


<!-- 
## 管理模块。
- 该模块允许管理员角色将智能合约部署到以太坊网络中。
- 该模块还包括开放和锁定注册以及允许参与者退出等功能。
## 访问控制模块
- 可验证用户在应用程序中的角色，
- 决定是否执行相应的模块或功能。
## 义务模块
- 负责收集各种义务记录，
- IPM防止推理模块现在已在 TAB 的去中心化信任设置中的智能合约中部署
- 因此可以防止在保护隐私的应用中进行推理攻击。
## 检查模块
- 可让授权用户检查不当行为或恶意活动。
## 激励模块
- 协调上述模块，利用以太坊网络的支付功能对用户进行奖励或惩罚。
概括地说,m个数据用户需要平均支付为自己以及n个数据所有者和第三方审计方(TPA)调用注册函数的费用。也就是说:- 有m个需要访问数据的用户。- 有n个拥有这些数据的数据所有者。- 还有一个第三方审计方(TPA)。- 每个数据用户都需要调用注册函数,向系统注册。- 调用注册函数需要支付一定的Gas费用。- m个数据用户需要平均支付调用所有m+n+1个实体(包括m个用户,n个所有者,1个TPA)的注册函数所需要的整体Gas费用。- 这样可以平分注册的总体费用,避免只有数据用户支付费用的情况。总结一下,这个设计可以让多个受益方均分注册函数调用的费用,而不是只让数据用户承担所有费用,这样更加公平合理。Gas费用的分担方式也提高了整个系统的可持续性
- 这样通过注册费、日志费、保证金以及监测的机制设计,可以有效抑制各方的不当行为,保证系统的公平与可靠
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# TAB Procedures

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_30_38_20231016113038.png" class="mx-auto" />

<!-- 
1. 在实体初始化的第一阶段，框架中的每个实体都会生成公钥和私钥对，注册其角色，并将其标识符和带有签名的公钥绑定发布到 BTABSC
2. 在第二阶段，TPA 通过设置主公钥和私钥对、为所有实体生成通用公钥并将绑定及其签名发布到 BTAB SC 来初始化 FE 密码系统。
3. 第三阶段，每个数据所有者选择一个随机数作为密钥服务标识符，并向 TPA 请求实体特定的公钥。 -TPA 为数据所有者生成公钥，并发布响应密钥服务快照以履行其密钥服务审计义务。 -然后，数据所有者使用公钥对其数据进行加密，并发布收到的公钥的收据。
4. 在第 IV 阶段，数据用户对加密数据应用产品内部功能，并向 TPA 请求功能解密密钥以及密钥服务标识符和密钥服务快照
-->

---
id: 3
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Applicability of TAB

<br>

**TAB is applicable to ABE-based applications by replacing the following audit obligations:**

$$
\pmb{\mathcal{S}_{\mathrm{req}}^{\mathcal{C}_{j}^{\mathrm{user}}}=\langle r^{\prime},\boldsymbol{y}_j,t_{\mathcal{C}_{j}^{\mathrm{user}}},\mathrm{Sig}_{\mathrm{sk}_{\mathcal{C}_{j}^{\mathrm{user}}}}(r^{\prime},\boldsymbol{y}_j,t_{\mathcal{C}_{j}^{\mathrm{user}}})\rangle,}
$$

$$
\pmb{\mathcal{S}_{\mathrm{resp}}^{\mathcal{A}}=\langle r^{\prime},\mathrm{H}(\mathrm{sk}_{\boldsymbol{y}_{j}}^{\mathrm{FE}}),t_{\mathcal{A}},\mathrm{Sig}_{\mathrm{sk}_{\mathcal{A}}}(r^{\prime},\mathrm{H}(\mathrm{sk}_{\boldsymbol{y}_{j}}^{\mathrm{FE}}),t_{\mathcal{A}})\rangle,}
$$

**by the corresponding audit obligations:**

$$
\pmb{\mathcal{S}_\mathrm{req}^{\mathcal{C}_j^{\mathrm{user}}}=\langle r^{\prime},S_j,t_{\mathcal{C}_j^{\mathrm{user}}},\mathrm{Sig}_{\mathrm{sk}\mathcal{C}_j^{\mathrm{user}}}(r^{\prime},S_j,t_{\mathcal{C}_j^{\mathrm{user}}})\rangle,}
$$

$$
\pmb{\mathcal{S}_{\mathrm{resp}}^{\mathcal{A}}=\langle r^{\prime},\mathrm{H}(\mathrm{sk}_{\mathcal{S}_{j}}^{\mathrm{ABE}}),t_{\mathcal{A}},\mathrm{Sig}_{\mathrm{sk}_{\mathcal{A}}}(r^{\prime},\mathrm{H}(\mathrm{sk}_{\mathcal{S}_{j}}^{\mathrm{FE}}),t_{\mathcal{A}})\rangle}
$$

<!--  

-->

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Security Guarantee

> - ***Log-Consistency***
> - ***Unforgeable-Service***
> - ***Non-Fabrication***

<br>

# Privacy Guarantee
> - ***ABE, FE, and multi-key HE***
> - ***Without any privacy-sensitive information***

<br>

# Trustworthiness Goal
> - ***Deploy IPM in the Smart Contract***

<!--  
## 日志一致性(log-consistency):
区块链的交易历史具有不可篡改性,任何试图修改或回滚历史记录的行为都会被网络检测并拒绝。这保证了公共账本的完整性。
## 不可篡改服务(unforgeable-service):
区块链网络中的参与方无法伪造或伪装他们没有的服务。例如cannot forge a signature without the corresponding private key。这提高了系统的可信度。
## 不可伪造(non-fabrication):
区块链系统具有可审计和可追溯的操作记录,参与方不能伪造或篡改记录来欺诈或互相指责。这保证了系统的公平性。综上,这三个属性确保了区块链作为公共账本的可靠性、不可篡改性和可审计性,是区块链能够实现分布式信任的基础。它们共同增强了整个系统的安全性与可信度。

- TAB不仅可以应用到ABE场景,也可以应用到基于功能加密(FE)或多密钥同态加密(multi-key HE)的计算应用中,来实现隐私保护。
- 对于 FE 或多钥匙 HE 中的身份没有任何隐私担忧，因为这些身份可以是任何独特的字符，没有任何隐私敏感信息。
- 此外，TAB 框架只接收基于 ABE 的应用程序中属性标识符的哈希值，而不接收潜在的敏感属性信息。因此，此类账户标识符或审计材料的哈希值不会泄露任何私人可识别信息

- 每个不诚实的实体都需要发布密钥服务快照，以证明自己已经履行了公开参数分发和私钥服务的义务。
- IPM 被部署在智能合同中，在公开可审计的环境中自动执行，从而增加 IPM 的透明度和可信度
-->

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Implemented Smart Contract

<br>

#### **Programming Language**

> *Solidity*<br>

<br>
<br>

#### **Development Environmen**

> *Truffle*

<br>
<br>

#### **Test Framework and Asset Pipeline**

> *Ethereum Virtual Machine*

<!--  

-->

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Function types

- #### **Administrative and Incentive Functions**
> $\mathcal{transferOwnership(newOwner)}$ & $\mathcal{renounceOwnership()}$

- #### **Registration Functions**
> *Focus on the initialization phases of TAB*

- #### **Obligation Functions**
> *Request Snapshots & Response Snapshots*

- #### **Inspection Functions**
> $\mathcal{inspectObligationKS()}$ & $\mathcal{inspectObligationPP()}$

<!--  
1. 这两个函数分别允许转移合约的所有权和让合约没有所有者。此外，我们还定义了几个提款和存款功能，有助于建立一个基础的激励和惩罚机制。
2. 注册功能主要集中在TAB的初始化阶段（即，第一阶段和第二阶段，如第3.3.3节所示，每个实体都可以注册一个角色，并在区块链中发布其身份到公钥的绑定。
3. 义务功能涉及 TAB 模型的核心特征, 具体来说，"recordKSPKReq "和 "recordKSSKReq "允许行为体发布关键服务请求快照，而 "recordKSPKResp "和 "recordKSSKResp "则允许 TPA 记录相应的关键服务响应快照。然后，"recordKSPKResp "函数允许我们确认是否收到了密钥服务。
4. 检查功能针对记录的审计义务的监督任务, 具体来说，"inspectObligationKS "允许自动检查密钥服务义务的完整性，而 "inspectObligationPP "则允许监控者验证已发布的身份与公钥绑定。在激励设计方面，如果检测到不诚实行为，相应实体将被处以固定数量的以太币罚款，这些以太币将作为激励奖励提供给监控者。
-->

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Experimental Setup

Experimental hardware
> - *Macbook Pro platform* 
> - *2.3GHz 8-Core Intel Core i9 processors*
> - *32GB DDR4 memory*

Test Network
> *The Ethereum official test network, Rinkeby*

Test Cases
> - *Automated testing framework of Truffle*
> - *Built on Mocha*


<!--  
具体来说，为了进行演示，我们使用五个以太坊账户来模拟 TAB 中的各种实体，即管理员、TPA、数据所有者、数据用户和监控者的角色。针对各种场景，我们编写了相应的测试用例来评估性能（即行政、注册、义务等场景的气体成本和时间成本）。
-->

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>

# Experimental Results

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_17_8_38_20231016170838.png" class="mx-auto" />

<!--  
- 我们在表 2 中报告了 TAB 在不同测试场景下对选定功能的性能表现。其中，性能包括两个方面：Gas成本和测试时间。
- 如表 2 所示，大多数功能的成本都很低。具体来说，除智能合约部署外，各项功能的成本一般都在 10^5 Gas的水平。
- 关于调用最多的义务和检查功能，为记录一项关键服务的审计义务，与三阶段承诺相关的功能（即记录 KSSKReq、记录 KSSKResp、记录 KSConfirm）分别花费了 43173 、84211 、43402 Gas。
- Ks和PP审核义务的检查成本分别为 24511 和 37842 Gas。
- 还测量了测试选定函数所需的时间。除Administrative外，其余功能的调用时间均小于 100 毫秒。
- 测试时间与执行时间有关，而不是与确认交易的时间有关，所以智能合约的部署时间仅为 183 毫秒，而不是一般的交易确认时间（约 6 分钟）。
-->

---
id: 4
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>
<br>

# Framework’s Scalability

<mimage layout="r" url="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/16_11_36_40_20231016113640.png" class="right-10 absolute" width="500" />

<br>

#### **Federated learning**
> Built on the FE cryptosystem<br> with a TPA for key service

<br>

#### **Enrolled Data Owners**
> Increased from 6 to 10

<br>

#### **Train a CNN Model**
> Over MINST dataset

<!--  
- 由于 TAB 只关注用户与 TPA 之间的关键交互，与 FL 培训的时间成本相比，时间成本可以忽略不计
- 如图所示，引入TAB框架对原有隐私保护联邦学习训练时间影响很小。
- 参与者数量增加会影响隐私保护应用(联邦学习)的时间
- 但对TAB时间影响不明显
-->

---
id: 5 
---

<img src="https://gitlab.com/Sh3ldon/MyPic/-/raw/main/pictures/2023/10/15_16_48_51_DMU.png" class="top-5 right-5 absolute" width="80" />

<br>
<br>

# Conclusion

<br>

- #### **Proposing TAB framework for TPA transparency**

<br>

- #### **Applying to modern privacy-preserving cryptography applications**

<br>

- #### **Using Ethereum blockchain as public ledger**

<br>

- #### **Novel smart contract for accountability with incentives**

<br>

- #### **Evaluation shows efficiency, security and privacy of TAB**