---
timezone: UTC+8
---

# Max

**GitHub ID:** Max-wht

**Telegram:** 

## Self-introduction

Web3 实习计划 2025 冬季实习生

## Notes

<!-- Content_START -->
# 2026-01-12
<!-- DAILY_CHECKIN_2026-01-12_START -->
### **\[B-1\] Etherscan::Transaction**

**Description** 对于ETH来说，区分交易的类别是很重要的。

**\[Transaction type classification\]**

-   **🛜Type0 \[Legacy Transaction\]**
    
    最早的以太坊交易形式，使用 **单一 Gas Price**，没有 Base Fee / Priority Fee 的概念，手续费 = `Gas Used × Gas Price`，现在仍然**兼容**，但不推荐使用。这也是很多链下服务出bug的一个点，协议太老了，不适配新协议。下面的表格着重看gasPrice和gasLimit
    
    | 字段 | 说明 |
    | --- | --- |
    | gasPrice | 固定 gas 单价 |
    | gasLimit | Gas 上限 |
    | nonce | 交易序号 |
    | to | 接收地址 |
    | value | ETH 数量 |
    | data | 合约数据 |
    
-   🛜 **Type1 \[Access List Transaction (EIP-2930)\]**
    
    核心概念是AccessList，这个会直接声明要访问的数据
    
    ```
    [
      {
        address: 0xContractA,
        storageKeys: [slot1, slot2, ...]
      },
      {
        address: 0xContractB,
        storageKeys: [...]
      }
    ]
    ​
    ```
    
-   🛜 **Type 2：EIP-1559 Transaction (主流)**
    
    引入 **Base Fee（销毁）**，引入 **Priority Fee（矿工小费）**，自动退还多余 Gas
    
    ```
    effectiveGasPrice =
    min(
      maxFeePerGas
      baseFee + maxPriorityFeePerGas
    )
    ```
    
    | 字段 | 含义 |
    | --- | --- |
    | maxFeePerGas | 你愿意支付的最高 Gas |
    | maxPriorityFeePerGas | 给矿工的小费 |
    | baseFee | 网络自动决定 |
    
    相当于原来的`gasPrice`被拆分成了`maxFeePerGas`和`maxPrioityFeePerGas`，实际的gas Fee
    
-   🛜 **Type 3：Blob Transaction（EIP-4844 / Proto-Danksharding）**
    
    2024年引入，面向layer2，数据放在blob中，隔一段时间主网会删除Blob
    
    Rollup（如 Arbitrum、Optimism）提交数据，数据放在 **Blob** 中，而不是 calldata，极低的数据成本，不直接参与 EVM 执行，专为扩容设计。给 Rollup（如 Arbitrum、Optimism）提交数据，数据放在 **Blob** 中，而不是 calldata。极低的数据成本，不直接参与 EVM 执行，专为扩容设计
<!-- DAILY_CHECKIN_2026-01-12_END -->
<!-- Content_END -->
