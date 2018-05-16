# admin
# **MGR**

README
-----------------------------------------------------------------------------------------------------------------------
MGR.sol is a fixed supply contract with a fixed supply of 110000000 initially assigned to the owner of the contract.

The Contract is based on ERC20 Token Standard.

The code is written for Solidity version 0.4.21

## What is this repository for?

MGR ICO contract.

## Coin specifications:

Token name - Mapplegreen

Token Symbol - MGR

Decimals allowed - 8

MGR Token Total Supply - 110000000

## How Does A Bitcoin MGR Contract Work?

Deploy the above MGR.sol smart contract and obtain its address. The address which contains Smart Contact deployed the Smart Contract becomes the Owner of the Smart Contract.

## Token Balance

To check the token balance of token holder, balanceOf() function needs to be used. For example, assume the MGR contract has two token holders:

0xaaa with a balance of 500 MGR
0xbbb with a balance of 100 MGR
## The balanceOf() will return following values:

balanceOf(0xaaa) will return 500
balanceOf(0xbbb) will return 100
## Transfer Token 
To transfer MGR tokens to different address, transfer() function needs to be used.

For example,If 0xaaa wants to transfer 100 MGR to 0xbbb, 0xaaa will execute the transfer function:

transfer(0xbbb, 100)
The balanceOf() will now return following values:

balanceOf(0xaaa) will return 400
balanceOf(0xbbb) will return 200
## Approve and TransferFrom Token Balance
If 0xbbb wants to authorise 0xaaa to transfer some tokens on his behalf, then 0xbbb will execute the approve() function

For example,If 0xbbb wants to approve 50 MGR to 0xaaa, 0xbbb will execute the function:

approve(0xaaa, 50)
The approve data structure will now contain the following information:

allowed[0xbbb][0xaaa] = 50
Now, if 0xaaa wants to later transfer some tokens from 0xbbb to itself, then 0xaaa will execute transferFrom() function

For example, if 0xaaa wants to transfer 20 MGR to itself, 0xaaa will execute function:

transferFrom(0xbbb, 0xaaa, 50)
The balances data structure will contain the following information:

balances[0xaaa] = 450
balances[0xbbb] = 150
And, approve data structure will now contain the following information:

allowed[0xbbb][0xaaa] = 50
Thus, 0xaaa can still spend 10 MGR from 0xbbb,

The balanceOf() will now return following values:

balanceOf(0xaaa) will return 450


The above two addresses(0Xaaa, 0Xbbb) taken in Example are not Valid Address, to make transaction you need to have a valid Ethereum Address.
