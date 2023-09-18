# 💱 Token Swap

Jur’s runtime includes a pallet to migrate tokens from VeChainThor (an EVM compatible chain) towards the new Substrate-based Jur Chain.

The swap is achieved by the means of a one-way token lock.

On the VeChain side a traditional deposit contract locks $JUR in it.

On the Jur Chain side tokens can be claimed provided that the VeChain state root is fed into our runtime in order to be able to access the storage and provided that related proofs of deposits are provided.

A message signed on the VeChain side will provide the new Substrate address that can claim $JUR.

The state root can be updated via Root Origin.

\
Jur has modified the original VeChain [thor](https://github.com/vechain/thor) binary to expose some data useful to generate proofs in a similar fashion to what eth\_getProof does in the Ethereum context. This data is all provided by thor; endpoints are just exposing them in a way that’s easy to interact with for the purpose of the token swap. Changes are visible in the following [commit](https://github.com/jurteam/thor/commit/2300537eaddd1126839415642427fb9131784e59).
