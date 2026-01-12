---
timezone: UTC+8
---

# Kevin Jiang

**GitHub ID:** doctorzero666

**Telegram:** @ZE_Monster

## Self-introduction

Web3 实习计划 2025 冬季实习生

## Notes

<!-- Content_START -->
# 2026-01-12
<!-- DAILY_CHECKIN_2026-01-12_START -->
# **今日学习总结（以太坊 / DeFi / Uniswap / Compound / NFT）**

### **1）以太坊基础原理：它到底是什么？**

-   **以太坊 = 一台全世界共同维护的“公共电脑”**
    
    大家都运行同一套规则，所以你在上面做的事情（转账、交易、发 NFT）都会被记录在链上，任何人都能验证。
    
-   **账户有两种：**
    
    -   **EOA（外部账户）**：用钱包（比如 MetaMask）控制的地址，能发起交易。
        
    -   **合约账户**：智能合约的地址，只能被交易触发后按代码执行。
        
-   **Gas（手续费）是“让机器干活的电费”**
    
    每次操作（转账、调用合约、mint NFT）都要消耗计算资源，所以要付 gas。网络越忙，gas 越贵。
    

* * *

### **2）DeFi：去中心化金融是怎么回事？**

-   **DeFi = 把传统金融的“借贷/交易/理财”搬到链上**
    
-   今天接触的两类 DeFi：
    
    -   **去中心化交易（DEX）**：代表是 Uniswap（换币）
        
    -   **借贷协议（Lending）**：代表是 Compound（存币赚利息、抵押借币）
        

* * *

### **3）Uniswap：不用“买卖双方撮合”，也能交易**

-   传统交易所像“菜市场撮合”：有人挂买单、有人挂卖单，匹配成交。
    
-   **Uniswap 像“自动售货机”**：你把一种币塞进去，机器按规则吐出另一种币。
    
-   它的核心是 **AMM（自动做市商）+ 流动性池（Liquidity Pool）**：
    
    -   池子里放着两种币（比如 ETH/USDC）
        
    -   价格由池子里两种币的比例决定
        
-   **一个重要概念：滑点（Slippage）**
    
    -   换得越多，池子比例被“推得越高”，价格就越不划算
        
    -   所以“大额兑换”通常滑点更明显
        

* * *

### **4）Compound：存币、借币怎么自动化的？**

-   **Compound = 链上“借贷市场”**
    
-   两种最常见动作：
    
    -   **Supply（存入）**：把币存进去，赚利息（利息来自借款人）
        
    -   **Borrow（借出）**：抵押资产，借出另一种资产
        
-   **关键逻辑：超额抵押**
    
    -   你想借钱，得先押一笔更值钱的资产
        
    -   如果抵押物价格跌太多，会触发 **清算（Liquidation）**（系统强制卖掉你的抵押物来还债）
        

* * *

### **5）NFT：它和“普通代币”最大的区别**

-   **NFT = 独一无二的链上“所有权凭证”**
    
-   大白话对比：
    
    -   **ERC-20 代币**：每个都一样
        
    -   **NFT（ERC-721 / ERC-1155）**：每个都不一样（像身份证编号/门票编号）
        
-   NFT 本质不一定是“图片”，更像：
    
    -   一条链上记录：谁拥有它
        
    -   +（可选）指向图片/文件的链接（很多存在 IPFS/中心化服务器上）
        

* * *

### **6）实操记录：我今天在链上真正做了什么**

-   ✅ **领取 SepoliaETH 测试币（Faucet）**
    
    ![image.png](https://raw.githubusercontent.com/IntensiveCoLearning/Web3_Internship_Bootcamp_2026_Winter/main/assets/doctorzero666/images/2026-01-12-1768221565468-image.png)
    
    用测试网模拟真实操作：不用真钱，但流程和主网很像。
    
-   ✅ **第一次转账（测试网转账）**
    
    体验了交易的关键要素：地址、金额、gas、等待确认。
    
-   ✅ **第一次做 NFT（Mint）**
    
    ![image.png](https://raw.githubusercontent.com/IntensiveCoLearning/Web3_Internship_Bootcamp_2026_Winter/main/assets/doctorzero666/images/2026-01-12-1768221538545-image.png)

* * *

## **我今天最大的收获：**

我把 Web3 从“概念”变成了“亲手做过一次”：

**我知道以太坊怎么记账（gas/交易/合约），也知道 DeFi 两大应用（换币 Uniswap、借贷 Compound），并且我在测试网完成了领币、转账、mint NFT 的完整闭环。**
<!-- DAILY_CHECKIN_2026-01-12_END -->
<!-- Content_END -->
