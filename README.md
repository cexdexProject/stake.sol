




CexDexStaking
A simple Ethereum smart contract for staking ERC20 tokens.

Overview
The CexDexStaking contract allows users to stake a specified ERC20 token and keep track of their staked balances. Users can stake or withdraw tokens anytime they wish.

Key Features
Staking: Users can stake their tokens in the smart contract.
Withdrawal: Users can withdraw their staked tokens.
Balance Query: Users can check the number of tokens they have staked.
Events: The contract emits events for staking and withdrawing activities for better transparency.
Interfaces
IERC20
An interface representing the required functions of an ERC20 token that will be used for staking.

CexDexStaking
The main contract where users can stake their tokens.

Functions
stake(uint256 amount)
Allows users to stake a specified amount of tokens.
Emits a Staked event.
withdraw(uint256 amount)
Allows users to withdraw a specified amount of their staked tokens.
Emits a Withdrawn event.
balanceOf(address user)
Returns the staked token balance of a specified user.
Events
Staked(address indexed user, uint256 amount)
Emitted when a user successfully stakes tokens.

Withdrawn(address indexed user, uint256 amount)
Emitted when a user successfully withdraws their staked tokens.

Requirements
stakingToken: The ERC20 token that users will stake. This is set in the constructor when deploying the contract.

