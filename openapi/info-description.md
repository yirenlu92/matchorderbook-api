# Introduction

MEP Orderbook provides a decentralized way to transfer assets between chains that can theoretically exchange all idle resources and support all coins. 

The MEP Orderbook works as follows:

- The user creates an order to transfer a certain number of tokens from chain A to chain B and offers to pay a certain reward
- MEP Orderbook locks the tokens to be transferred as well as the reward
- MEP Orderbook displays the user's order on the page
- When the order taker sees the order, if he/she finds the reward attractive and has the desired token, he/she can choose to take the order
- The order taker will transfer the specified token on chain B to the order maker via MEP Orderbook.
MEP will collect the transaction message and consensus to determine that the order taker has actually transferred tokens to the order maker on Chain B
- The order taker can then request MEP to issue proof of successful transfer
- With this credential, the order taker can go to chain A and take out the token and reward pledged by the order maker.

# Getting Started

## 1. Call `/orders` to get all fresh orders

## 2. Call `/takeorder` to take the order

## 3. Call the `takeOrder()` method of the deployed contract on the dest chain, this will transfer tokens from taker to orderMaker

## 4. Call `withdrawall` to get one signature from the backend

## 5. Call the `withdrawall()` method of the deployed contract on the src chain to withdraw all tokens that the taker can get back

