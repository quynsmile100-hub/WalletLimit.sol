# WalletLimit.sol
WalletLimit.sol
pragma solidity ^0.8.20;
contract WalletLimit {
    function deposit() public payable {
        require(msg.value <= 1 ether, "Too much");
    }
}
