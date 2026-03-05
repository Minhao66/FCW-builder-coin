// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";

contract BuilderCoin is ERC20, Ownable {
    constructor() ERC20("BuilderCoin", "BDC") Ownable(msg.sender) {
        // 初始铸造 1,000,000 个代币给自己（部署者）
        _mint(msg.sender, 1000000 * 10 ** decimals());
    }

    // 只有 owner 可以额外铸造代币给任意地址
    function mint(address to, uint256 amount) public onlyOwner {
        _mint(to, amount);
    }

    // 只有 owner 可以销毁自己的代币
    function burn(uint256 amount) public onlyOwner {
        _burn(msg.sender, amount);
    }
}
