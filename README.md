# ERC1363_Token
Implementation for the ERC-1363 Tokens

ERC-1363 allows to implement an ERC-20 token that can be used for payments.

This is an implementation of the ERC-1363 Payable Token that defines a token interface for ERC-20 tokens that supports executing recipient code after transfer or transferFrom, or spender code after approve.

Abstract
There is no way to execute code after an ERC-20 transfer or approval (i.e. making a payment), so to make an action it is required to send another transaction and pay GAS twice. ERC-1363 makes token payments easier and working without the use of any other listener. It allows to make a callback after a transfer or approval in a single transaction.

There are many proposed uses of Ethereum smart contracts that can accept ERC-20 payments.

Examples could be:

to create a token payable crowdsale
selling services for tokens
paying invoices
making subscriptions

Anyway you can use it for specific utilities or for any other purposes who require the execution of a callback after a transfer or approval received.
