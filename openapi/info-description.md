# Introduction

Welcome to the MEP Orderbook documentation. We offer complete a REST API for your algorithmic trading needs.

# Getting Started

## Market Makers



## Market Takers

To take an order programatically, follow these steps:

1. Call `/orders` to get all fresh orders	
2. Call `/takeorder` to take order specified by order id and taker address. This call should return the result and one signature.
3. Call the `takeOrder()` method of the deployed contract on the dest chain, which will transfer tokens from taker to orderMaker
4. Call `/withdrawall` to get a signature from the backend
5. Call the `withdrawall()` method of the deployed contract on the src chain to withdraw all tokens that the taker can get back


# Rest API

We offer a HTTP-based API with full orderbook functionality.

Requests and responses use JSON.

# Authentication

# Rate Limits
