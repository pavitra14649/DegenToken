# DegenToken Contract

The `DegenToken` contract is an ERC20 token with additional features for a gaming platform. It allows for minting, transferring, and burning tokens, as well as redeeming tokens for in-game items (cards).

## Features

- **Mint Tokens:** Allows the owner to mint new tokens for buyers in a queue.
- **Transfer Tokens:** Allows users to transfer tokens to other users.
- **Redeem Cards:** Users can redeem tokens for different types of in-game cards.
- **Burn Tokens:** Allows users to burn their own tokens.
- **Check Balance:** Users can check their token balance.

## Contract Details

- **Solidity Version:** ^0.8.24
- **SPDX-License-Identifier:** MIT

## Functions

### `addBuyerToQueue`


    function addBuyerToQueue(address _walletAddress, uint256 _tokenAmount) public


## Parameters:
 _walletAddress: The address of the buyer.
 _tokenAmount: The amount of tokens to be purchased.

 ## mintTokens

function mintTokens() public onlyOwner

## transferTokens

    function transferTokens(address _recipient, uint256 _amount) public

Transfers tokens from the sender's account to the recipient's account.

## redeemCard

    function redeemCard(CardTypes _cardType) public
Redeems tokens for a specified type of card.

## burnTokens

    function burnTokens(address _holder, uint256 _amount) public
Burns tokens from the specified holder's account.

## checkTokenBalance

    function checkTokenBalance() public view returns (uint256)
Returns the token balance of the caller.

## Redeemable Cards
The contract includes an enumeration of card types:

Common

Uncommon

Rare

Epic

Legendary

Users can redeem tokens for these cards, which will be recorded in their PlayerInventory.
## License
This project is licensed under the MIT License.
