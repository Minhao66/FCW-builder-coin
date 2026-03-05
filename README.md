# FCW Builder Coin

**FCW** = Future Chain World  
这是我从零基础重新写的第一个 ERC-20 代币合约，彻底抛弃之前的所有旧版本和混淆问题，代表我正式进入链上 builder 阶段。

## 项目信息
- **Token 全称**：FCW Builder Coin  
- **符号**：FCW  
- **精度**：18 decimals  
- **初始供应**：1,000,000 FCW（部署时全部 mint 给 owner）  
- **合约地址**：0x44AeeeC1579CcC010969a8C7FcD30764A4c445c5 (Sepolia 测试网)  
- **Etherscan**：https://sepolia.etherscan.io/address/0x44aeeec1579ccc010969a8c7fcd30764a4c445c5  
- **源码验证**：已 Verify（公开透明，可查完整代码）

## 核心功能
- 标准 ERC-20（转账、余额查询、授权等）
- Ownable 权限控制：只有 owner（部署者）可以额外 mint / burn
- 已测试：
  - 初始 mint：1,000,000 FCW
  - burn：成功销毁部分代币（余额减少）
  - mint：成功额外增发（余额增加）

## 学习收获
- 彻底掌握了“清理旧实例 → 新文件 → 部署 → At Address 加载 → 测试闭环”的全流程
- 理解 _mint / _burn 内部逻辑、onlyOwner 修饰符、decimals 处理
- 学会避免合约混淆、每次新功能最好重新部署验证

## 下一步计划
- 添加 pause / unpause（暂停转账）
- 开发简单前端 dApp（查余额 + 转账）
- 参与 Gitcoin 小型 bounty（从文档/内容类入手）
- 探索更多标准：ERC-721、升级代理合约

欢迎任何反馈、fork、star 或合作！  
持续学习、持续构建中。  
@Minhaonb66 | Web3 Builder Journey  
最后更新：2026 年 3 月
