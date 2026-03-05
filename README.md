FCW Builder Coin —— 从“只会领水”到自己铸币的第 N 天

名字 FCW = Future Chain World  
这是我从零基础重新写的 ERC-20 代币，彻底抛弃之前混淆的旧版本，重新部署、重新测试。

核心信息：
- 符号：FCW
- 初始供应：1,000,000（已 mint 给自己）
- 合约地址：0x44AeeeC1579CcC010969a8C7FcD30764A4c445c5 (Sepolia)
- 功能：ERC-20 标准 + onlyOwner 的 mint & burn
- GitHub + 源码：https://github.com/Min
- ## 测试记录
- burn 成功：销毁 10 FCW
- mint 成功：额外铸造 50 FCW​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​​
- ## 学习收获
- 彻底掌握了部署新版本避免混淆的方法
- 理解 _burn 和 _mint 的内部逻辑
- 会用 Remix 的 At Address 加载已部署合约
