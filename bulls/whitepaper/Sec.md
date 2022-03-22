# Security

The contract itself is highly important to us and we didn’t do a script kiddie approach here nor a fork of another contract. We will continue to work with security-focused Blockchain and Solidity developers to overlook our code and intent before putting anything in production. To further increase security on the funds on the project, they will be moved into cold wallets right after the Public sale and will then be invested into projects. Money is then strategically funded back into the contract and the owners will call the reward function to reward the The Ranch Bulls NFTs.

Picking the winners has been a no-brainer from the very beginning of this project. We have run thousands of tests (we come from a DevOps background) to show each The Ranch Bulls holder truly has a fair chance to be rewarded. Many contracts utilize pseudorandom numbers by using a keccack256 (hashing algorithm) to look at the block.timestamp and the block.difficultly to derive winners. The problem with this approach is that keccack256 will always hash the data the same way and the data it is hashing is predictable, thus it won’t create truly random outputs. To combat this problem, Chainlink has built a solution to request and receive random numbers from their VRF protocol.

[https://chain.link/chainlink-vrf](https://chain.link/chainlink-vrf)

Chainlink VRF (Verifiable Random Function) is a provably fair and verifiable random number generator (RNG) that enables smart contracts to access random values without compromising security or usability. This protocol also played a pivotal part in deciding on which blockchain we would deploy the project on as Polygon is one of the few supported blockchains and the cheapest way to interact back with Chainlink to request these random numbers each week.
