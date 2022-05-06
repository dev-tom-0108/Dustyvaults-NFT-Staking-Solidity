# Dustyvaults-NFT-Staking-Solidity
This is the NFT staking smart contract on BSC chain, the first project not to send NFT to the smart contract at all.

## Data Structure
```js
enum   Actions { UNSTAKED, FARMING }
struct Action  {
    address NFTAddress;
    uint256 NFTId;
    string hash;
    string name;
    uint256 timestamp;
    uint256 percent;
    uint256 reward; 
    uint256 amount;
    Actions action; 
} 
```

## Main Functions

Staking Function

```js
function stakebyHash(string memory hashx, string memory namex, address tokenAddress, uint256 tokenId, uint256 amount) external
```

Autoclaim Function

```js
function autoClaim(address addr, uint256 cid) external 
```

Unstake Function

```js
function unStake(address addr, uint256 cid) external
```
