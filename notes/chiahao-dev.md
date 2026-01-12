---
timezone: UTC+8
---

# chiahao-dev

**GitHub ID:** chiahao-dev

**Telegram:** 

## Self-introduction

Web3 实习计划 2025 冬季实习生

## Notes

<!-- Content_START -->
# 2026-01-12
<!-- DAILY_CHECKIN_2026-01-12_START -->
\# Web3 Day 1

\## 1. 阅读 Web3 实习手册 & 笔记整理

\### 求职相关技术栈

\#### 前端

\> 当前前端 Web3 开发中，\*\*Ethers.js / Web3.js 使用频率正在下降\*\*，主流逐渐转向 **Viem**

\- HTML5

\- CSS3

\- JavaScript (ES6+)

\- React / Vue

\- TypeScript

\- Next.js

\- Ethers.js / Web3.js / **Viem**

\#### 后端

\- Node.js / Go / Python

\- Viem / Web3.js / Ethers.js

\- RESTful API / GraphQL

\- MySQL / PostgreSQL

\- Docker / Kubernetes

\#### 智能合约

\- Solidity

\- Remix

\- Foundry / Hardhat

\- Phalcon / Tenderly

\- Yul

\---

\### 求职平台推荐

\#### 中文平台

\- **DeJob**：中文，大量高频 Web3 工作机会

\- **SmartDeer**：中文，综合性招聘平台

\- **电鸭社区**：中文，远程工作者社区

\#### 英文平台

\- **Web3Career**：专业的 Web3 招聘平台

\- **CryptoJobs**：区块链行业招聘信息

\- **The Ethereum Season of Internships**：以太坊实习季

\- **Ethereum Job Board**：ETH 生态旗舰项目招聘板

\---

\## 2. 智能合约开发模拟面试题

\### Q1. 智能合约开发遵循的范式？

**A1：**

\- **状态机模式**

智能合约本质上是一个状态机，通过交易推动状态迁移。

\- **事件驱动编程**

使用 `Event` 记录关键状态变化，便于前端监听和日志索引。

\- **模块化设计**

通过继承（Inheritance）和库（Library）实现代码复用和解耦。

\---

\### Q2. 常见攻击手段、原理与防护措施？

\#### 1️⃣ 重入攻击（Reentrancy Attack）

**攻击原理：**

1\. 合约向外部地址或合约发送 ETH`call`）

2\. 外部合约在回调中再次调用原合约函数

3\. 原合约尚未更新状态

4\. 攻击者反复进入函数，实现多次提款

**典型代码特征：**

\> ❌ 先转账，后更新状态

**防护措施：**

\- **CEI 模式（Checks → Effects → Interactions）**

\> ✅ 先更新状态，后进行外部调用

\- **重入锁（Reentrancy Guard）**

\- 使用 `bool locked` 作为互斥锁

\- 保证同一时间只能进入一次受保护函数

\---

\#### 2️⃣ 访问控制缺失（Access Control）

**攻击原理：**

\- 攻击者直接调用缺乏权限检查的敏感函数

**防护措施：**

\- 引入显式权限校验（如 `onlyOwner`）

\- 限制关键函数的调用者

**示例：**

\- `deposit()`：所有用户可调用

\- `withdraw()`：仅合约所有者可调用

\---

\#### 3️⃣ 整数溢出（Integer Overflow）

**背景：**

\- Solidity `v0.8.0` 之前默认不检查溢出

\- 数值超出范围会发生 **wrap around**

**攻击原理：**

\- 将变量推到 `2^256 - 1`

\- 再次递增 → 数值回绕到 `0`

\- 绕过条件检查，触发无限奖励逻辑

**防护措施：**

\- 使用 Solidity `>= 0.8.0`

\- 设置业务逻辑上的上限约束

\---

\### Q3. 交易生命周期（Transaction Lifecycle）

\#### 1️⃣ 签名与构造

\- 钱包收集字段：

\- `nonce`

\- `to`

\- `value`

\- `data`

\- `gasLimit`

\- `maxFeePerGas`

\- `priorityFeePerGas`

\- `chainId`

\- 使用私钥生成 `v, r, s`

\- RLP 序列化

\#### 2️⃣ 广播到 P2P 网络

\- 进入本地及邻居节点的 mempool

\- 节点按费用、nonce、gas 规则筛选

\#### 3️⃣ 打包区块

\- 验证者（PoS）选择高收益交易

\- 执行 EVM

\- 生成交易收据（Receipt）

\#### 4️⃣ 共识与传播

\- 区块包含新的 `stateRootreceiptsRoot`

\- PoS 下超过 2/3 验证者签名后 Finalize

\> ≈ 2 Epoch ≈ 64 Slot ≈ ~12 分钟

\#### 5️⃣ 确认数与终局性

\- 前端通常认为 `n ≥ 12` 确认足够安全

\- 最终由 Casper FFG 给出终局性（Finality）

\---

\## 3. Web3 实习计划（冬季）开营仪式回顾

（略）

\---

\## 4. 实践记录

\### 转账记录

\- Etherscan（Sepolia）：

[https://sepolia.etherscan.io/tx/0x60acd9c2ac47e204b3a5ea4fc7b269dbceda81cc24b182d30fc373dd10f73a02](https://sepolia.etherscan.io/tx/0x60acd9c2ac47e204b3a5ea4fc7b269dbceda81cc24b182d30fc373dd10f73a02)

\### NFT Mint

\- 完成 NFT Mint 体验

\---（哈哈哈）

![mfnft.png](https://raw.githubusercontent.com/IntensiveCoLearning/Web3_Internship_Bootcamp_2026_Winter/main/assets/chiahao-dev/images/2026-01-12-1768223172894-mfnft.png)

  
  
\## Review

今天是开营第一天，由于时差原因，实际学习内容不多。

计划明天重新规划时间安排，并逐步适应时差。
<!-- DAILY_CHECKIN_2026-01-12_END -->
<!-- Content_END -->
