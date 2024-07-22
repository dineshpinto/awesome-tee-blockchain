# Awesome TEE Blockchain

A curated list of resources for learning about Trusted Execution Environments (TEEs) in the context of blockchains. This list includes articles, research papers, code repositories, videos, and more.

## What are TEEs?

Trusted Execution Environments (TEEs) are secure areas within a main processor that ensure the integrity and confidentiality of the code and data loaded inside. TEEs provide a higher level of security than the normal execution environment by isolating the execution of sensitive applications and data from the rest of the system.

In the context of blockchains, TEEs are primarily used to enhance compute and data storage capabilities, ideally with minimal compromise to security, verifiability and decentralization.

Key characteristics of TEEs:

1. **Isolation**: TEEs separate sensitive code and data from the regular operating system and applications. This isolation helps protect against a wide range of attacks, including those from malicious software running on the main OS.

2. **Confidentiality and Integrity**: TEEs ensure that the data processed within them is protected from unauthorized access and tampering. This is crucial for sensitive operations such as cryptographic computations and handling confidential data.

3. **Secure Boot and Secure Storage**: TEEs support secure boot mechanisms to ensure that only authenticated and trusted code can be executed. They also provide secure storage for keys and other sensitive data.

4. **Attestation**: TEEs can generate cryptographic proofs (attestations) that confirm the authenticity and integrity of the code running within them. This allows external parties to verify that the TEE is running legitimate and unaltered code.

## Table of Contents

1. [Comparison](#comparison)
2. [Hardware](#hardware)
   - [Google Cloud Confidential Compute](#google-cloud-confidential-compute)
   - [Amazon Nitro](#amazon-nitro)
   - [AMD SEV](#amd-sev)
   - [Intel SGX](#intel-sgx)
   - [ARM](#arm-trustzone)
3. [Use Cases](#use-cases)
   - [Block Building](#block-building)
   - [General Compute](#general-compute)
   - [Privacy](#privacy)
4. [Repositories](#repositories)
   - [Rust](#rust)
   - [Go](#go)
   - [C++](#cpp)
   - [C](#c)
   - [Python](#python)
5. [Research Papers](#research-papers)
6. [Articles](#articles)
7. [Videos](#videos)

## Comparison

- [Blockchain Privacy and Security in Data Computation](https://www.zkon.xyz/blog/blockchain-privacy-mpc-zk-tee-explained)
- [4 Ways to Compare Trusted Execution Environments and Zero-Knowledge Proofs](https://oasisprotocol.org/blog/comparing-zkp-tee-privacy)

## Hardware

### Google Cloud Confidential Compute

- [Confidential Compute](https://cloud.google.com/blog/products/identity-security/introducing-google-cloud-confidential-computing-with-confidential-vms)
- [Confidential Accelerator for AI workloads](https://cloud.google.com/blog/products/identity-security/expanding-confidential-computing-for-ai-workloads-next24)
- [Confidential Space](https://cloud.google.com/docs/security/confidential-space)
- [Confidential VM attestation](https://cloud.google.com/confidential-computing/confidential-vm/docs/attestation)

### Amazon Nitro

- [Nitro](https://aws.amazon.com/ec2/nitro/)

### AMD SEV

- [SEV](https://www.amd.com/en/developer/sev.html)

### Intel SGX

- [SGX](https://www.intel.com/content/www/us/en/products/docs/accelerator-engines/software-guard-extensions.html)

### ARM TrustZone

- [TrustZone](https://www.arm.com/technologies/trustzone-for-cortex-m#:~:text=Arm%20TrustZone%20technology%20is%20used,to%20as%20the%20secure%20monitor.)

## Use Cases

### Block Building

- [The Future of MEV is SUAVE](https://writings.flashbots.net/the-future-of-mev-is-suave)
- [Block Building inside SGX](https://writings.flashbots.net/block-building-inside-sgx)
- [Running Geth within SGX: Our Experience, Learnings and Code](https://writings.flashbots.net/geth-inside-sgx)
- [SGX-Based Backrunning and Covert Channels](https://writings.flashbots.net/backrunning-private-txs-MPC#sgx-based-backrunning-and-covert-channels)
- [MEV-SGX -- A sealed bid MEV auction design](https://ethresear.ch/t/mev-sgx-a-sealed-bid-mev-auction-design/9677)

### General Compute

- [Automata Network](https://www.ata.network)
- [Phala Network](https://github.com/Phala-Network/phala-blockchain)

### Privacy

- [Oasis Protocol](https://oasisprotocol.org)
- [Secret Network](https://scrt.network)
- [How Secret Network Uses SGX](https://docs.scrt.network/secret-network-documentation/overview-ecosystem-and-technology/techstack/privacy-technology/intel-sgx/overview)

### Bridging

- [Avalanche Bridge: Secure Cross-Chain Asset Transfers Using Intel SGX](https://medium.com/avalancheavax/avalanche-bridge-secure-cross-chain-asset-transfers-using-intel-sgx-b04f5a4c7ad1)

## Repositories

### Rust

- [kata-containers/kata-containers](https://github.com/kata-containers/kata-containers) - Kata Containers is an open source project and community working to build a standard implementation of lightweight Virtual Machines (VMs) that feel and perform like containers, but provide the workload isolation and security advantages of VMs.
- [confidential-containers/guest-components](https://github.com/confidential-containers/guest-components) - Confidential Containers Guest Tools and Components
- [kinvolk/azure-cvm-tooling](https://github.com/kinvolk/azure-cvm-tooling) - Libraries and tools for Confidential Computing on Azure
- [HyperEnclave/hyperenclave](https://github.com/HyperEnclave/hyperenclave) - An Open and Cross-platform Trusted Execution Environment.
- [mobilecoinfoundation/mobilecoin](https://github.com/mobilecoinfoundation/mobilecoin) - Private payments for mobile devices
- [integritee-network/worker](https://github.com/integritee-network/worker) - ntegritee off-chain worker and sidechain validateer
- [capsule-corp-ternoa/ternoa-node](https://github.com/capsule-corp-ternoa/ternoa-node) - Ternoa's Node Implementation
- [automata-network/automata](https://github.com/automata-network/automata) - Automata Network is a modular attestation layer that extends machine trust to Ethereum with TEE Coprocessors.
- [Phala-Network/phala-blockchain](https://github.com/Phala-Network/phala-blockchain) - The Phala Network Blockchain, pRuntime and the bridge.
- [apache/incubator-teaclave-sgx-sdk](https://github.com/apache/incubator-teaclave-sgx-sdk) - Apache Teaclave (incubating) SGX SDK helps developers to write Intel SGX applications in the Rust programming language, and also known as Rust SGX SDK.
- [apache/incubator-teaclave](https://github.com/apache/incubator-teaclave) - Apache Teaclave (incubating) is an open source universal secure computing platform, making computation on privacy-sensitive data safe and simple.

### Go

- [google/go-tpm-tools](https://github.com/google/go-tpm-tools) - Go packages built on go-tpm providing a high-level API for using TPMs
- [matter-labs/vault-auth-tee](https://github.com/matter-labs/vault-auth-tee) - Hashicorp Vault plugin for authenticating Trusted Execution Environments (TEE) like SGX enclaves
- [usbarmory/GoTEE](https://github.com/usbarmory/GoTEE) - Go Trusted Execution Environment (TEE)
- [iotexproject/w3bstream](https://github.com/iotexproject/w3bstream) - An offchain computing layer for DePIN verifiable data computation, supporting a variety of validity proofs including Zero Knowledge (ZK), Trusted Execution Environments (TEE), and Multi-party Computation (MPC)
- [oasisprotocol/oasis-core](https://github.com/oasisprotocol/oasis-core) - Performant and Confidentiality-Preserving Smart Contracts + Blockchains
- [hyperledger/fabric-private-chaincode](https://github.com/hyperledger/fabric-private-chaincode) - FPC enables Confidential Chaincode Execution for Hyperledger Fabric using Intel SGX.

### CPP

- [microsoft/azure-tee-attestation-samples](https://github.com/microsoft/azure-tee-attestation-samples) - Trusted Execution Environment examples leveraging attestations on Azure
- [intel/linux-sgx](https://github.com/intel/linux-sgx) - Intel SGX for Linux
- [lsds/Teechain](https://github.com/lsds/Teechain) - Teechain: A Secure Payment Network with Asynchronous Blockchain Access
- [skalenetwork/sgxwallet](https://github.com/skalenetwork/sgxwallet) - sgxwallet is the first-ever opensource high-performance hardware secure crypto wallet that is based on Intel SGX technology. First opensource product on Intel SGX whitelist. Scales to 100,000+ transactions per second. Currently supports ETH and SKALE, and will support BTC in the future. Sgxwallet is under heavy development and use by SKALE network.
- [hyperledger-labs/private-data-objects](https://github.com/hyperledger-labs/private-data-objects) - The Private Data Objects lab provides technology for confidentiality-preserving, off-chain smart contracts.

### C

- [deislabs/mystikos](https://github.com/deislabs/mystikos) - Tools and runtime for launching unmodified container images in Trusted Execution Environments
- [openenclave/openenclave](https://github.com/openenclave/openenclave) - SDK for developing enclaves
- [mofanv/PPFL](https://github.com/mofanv/PPFL) - Privacy-preserving Federated Learning with Trusted Execution Environments
- [inclavare-containers/inclavare-containers](https://github.com/inclavare-containers/inclavare-containers) - A novel container runtime, aka confidential container, for cloud-native confidential computing and enclave runtime ecosystem.

### Python

- [ethernity-cloud/mvp-pox-node](https://github.com/ethernity-cloud/mvp-pox-node) - Ethernity Cloud Node

## Research Papers

- A. Nilsson, P. N. Bideh, and J. Brorsson, “A Survey of Published Attacks on Intel SGX” - [arXiv](http://arxiv.org/abs/2006.13598)
- K. Murdock, D. Oswald, F. D. Garcia, J. Van Bulck, D. Gruss, and F. Piessens, “Plundervolt: Software-based Fault Injection Attacks against Intel SGX” - [IEEE](https://ieeexplore.ieee.org/document/9152636)
- D. Natarajan, A. Loveless, W. Dai, and R. Dreslinski, “CHEX-MIX: Combining Homomorphic Encryption with Trusted Execution Environments for Two-party Oblivious Inference in the Cloud” - [Cryptology ePrint Archive](https://eprint.iacr.org/2021/1603)
- J. Lind, O. Naor, I. Eyal, F. Kelbert, P. Pietzuch, and E. Gun Sirer, "Teechain: A Secure Payment Network with Asynchronous Blockchain Access" - [arXiv](https://arxiv.org/abs/1707.05454)

## Articles

- [Verifiable Off-chain Compute - Florin Digital](https://florindigital.substack.com/p/verifiable-off-chain-compute-enabling)
- [Why trusted execution environments will be integral to proof-of-stake blockchains](https://venturebeat.com/datadecisionmakers/why-trusted-execution-environments-will-be-integral-to-proof-of-stake-blockchains/)
- [TEE-based Smart Contracts and Sealing Pitfalls](https://medium.com/initc3org/tee-based-smart-contracts-and-sealing-pitfalls-eccd5d751329)
- [Trusted Execution Environments and the Polkadot Ecosystem](https://polkadot.network/blog/trusted-execution-environments-and-the-polkadot-ecosystem)
- [Blockchains in Trusted Execution Environments (TEEs)](https://medium.com/@nadeem.bhati/blockchains-in-trusted-execution-environments-tees-9343b6c3f9e8)
- [Intel SGX and Blockchain: The iExec End-to-End Trusted Execution Solution](https://medium.com/iex-ec/iexec-end-to-end-sgx-solution-fee1e63297b2)
- [Blockchains + TEEs Day 1 Summary](https://decentralizedthoughts.github.io/2023-04-09-blockchainsplustees-day1-summary/)
- [Blockchains + TEEs Day 2 Summary](https://decentralizedthoughts.github.io/2023-04-17-blockchainsplustees-day2-summary/)
- [Intel SGX Explained](https://css.csail.mit.edu/6.858/2020/readings/costan-sgx.pdf)

## Videos

- [Private Smart Contracts are Worth the Price of the SGX - Andrew Miller](https://www.youtube.com/watch?v=L0bp6V1pn0s)
- [SGX Panel: Andrew Miller, Jonathan Passerat Palmbach, Phil Daian, Justin Drake](https://youtu.be/vokDXJmPCSI)
- [Enabling Cross Chain Transfers Using SGX](https://youtu.be/f2bU55ngO_c)
- [TEE for Blockchain Applications - Ari Juels](https://youtu.be/Xq7oWtiwWII?feature=shared)
- [Protected Order Flow - Flashbots](https://www.youtube.com/watch?v=v1TkocRScJg)
- [Blockchains + TEEs: Day 1](https://youtu.be/9-nhNQO5_Js)
- [Blockchains + TEEs: Day 2](https://youtu.be/zIU3gFTb2PM)
