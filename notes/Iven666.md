---
timezone: UTC+8
---

# Iven666

**GitHub ID:** Iven666

**Telegram:** @ivenlin666

## Self-introduction

Web3 实习计划 2025 冬季实习生

## Notes

<!-- Content_START -->
# 2026-01-12
<!-- DAILY_CHECKIN_2026-01-12_START -->
## 区块链基础概念

1.  去中心化和分布式网络很好，可是为什么会有人愿意提供这项服务呢？
    

因为他们会得到奖励 BTC。

-   网络服务提供商\\节点，提供网络服务，获得相应代币，如BTC。
    
-   比特币供应量有限，可以自由转账，具有天然货币属性。
    
-   比特币账户匿名，交易数据透明不可篡改，跨境结算方便，这些特性使得比特币具有了应用场景。
    
-   弊端：比特币具有不可追踪性，黑灰产交易盛行。
    

### 区块链运行过程

暂时无法在飞书文档外展示此内容  

![image.png](https://raw.githubusercontent.com/IntensiveCoLearning/Web3_Internship_Bootcamp_2026_Winter/main/assets/Iven666/images/2026-01-12-1768217086188-image.png)

### 区块链类型分类

| 区块链类型 | 节点加入方式 | 数据可见性 | 管理模式 | 适合场景 |
| 公链 | 任何人自由加入 | 所有人可见 | 去中心化（大家投票） | 加密货币、公共存证 |
| 联盟链 | 需联盟成员邀请/审批 | 仅联盟成员可见 | 多中心化（董事会决策） | 供应链、金融协作 |
| 私链 | 由老板严格审批 | 仅内部成员可见 | 中心化（老板说了算） | 企业内部管理、审计 |

### WEB3核心特征

-   数字主权属于用户
    
-   代码及法律，智能合约自动化执行
    
-   核心组件：
    

![image.png](https://raw.githubusercontent.com/IntensiveCoLearning/Web3_Internship_Bootcamp_2026_Winter/main/assets/Iven666/images/2026-01-12-1768217163723-image.png)

暂时无法在飞书文档外展示此内容

DAPP的核心应用创新：

-   数字资产真正属于用户
    
-   内容上链永远存在，无法被删除
    
-   Defi 协议可组合，乐高积木
    
-   降低金融门槛，无需银行卡，Defi无需KYC
    

## 去中心化的好与坏

### 好

-   信任成本降低，由智能合约代码自动执行约定，无需引入第三方
    
-   抗单点故障能力强，多节点结构
    
-   数字资产由用户自主管理，主权在民
    
-   生态开放，开发者可以在区块链网络上开发应用，创新技术和商业模式。
    

### 坏

-   公链节点众多，共识效率低下，吞吐量大，延时问题突出
    
-   用户体验不友好，私钥，钱包提高了准入门槛
    
-   安全问题，智能合约代码bug不能修改；DAO团队代币投票集中
    
-   法律合规问题。
    

## 以太坊

### 以太坊生态概览

1.  L1: 以太坊主网和 EVM账户系统（外部账户EOA和 合约账户CA）
    
2.  L2：OP和ZK 两种解决方案
    

-   OP：主要是optimism和arbitrum 两种方案。 OP是单轮欺诈验证，Arbi是多轮欺诈验证。Arbi的L1成本更低，安全性更高。
    
-   ZK：主要有 ZK技术细节就不懂了
    

当前主流可以分成 **三派**：

**EVM 等价派**：Scroll、Polygon zkEVM

**EVM 兼容派**：zkSync Era

**非 EVM 派**：Starknet

| 项目 | EVM 路线 | 技术风格 | 适合谁 |
| zkSync Era | 兼容 | 产品优先 | 应用开发 |
| Scroll | 等价 | 技术保守 | DeFi |
| Polygon zkEVM | 兼容 | 工程整合 | 生态项目 |
| Starknet | 非 EVM | 技术激进 | 长期主义 |

3.  SideChain:侧链现在没什么有价值的应用，忽略。
    

以太坊生态的几个层次需要介绍一下。

### 以太坊核心机制

1.  账户系统 EOA （用户账户，轻节点） CA（合约部署账户）
    
2.  GAS费模型：总费用 = Gas Limit × Gas Price。实习手册gas费模型没讲清楚
    

是什么：你愿意为每单位 Gas 支付多少费用（以 Gwei 计价，1 Gwei = 0.000000001 ETH）。这是一个由市场供需决定的价格。 Gas limit 就是你愿意支付的最多费用。

作用：决定了你的交易被处理的优先级。在网络拥堵时，更高的 Gas Price 能吸引矿工/验证者优先打包你的交易。

如果交易完成，实际 `Gas Used ≤ Gas Limit`，你只需支付 `Gas Used × Gas Price`，剩余部分退回。

如果执行中 `Gas Used` 达到 `Gas Limit` 但交易未完成，交易将失败并回滚，但已消耗的 Gas 不会退回（因为矿工已经付出了计算工作）。

-   EIP-1559升级后，Gas= Gas used\*( base fee + priority fee)
    

3.  EVM 以太坊虚拟机
<!-- DAILY_CHECKIN_2026-01-12_END -->
<!-- Content_END -->
