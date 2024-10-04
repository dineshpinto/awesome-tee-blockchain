# Awesome TEE Blockchain

A curated list of resources for learning about Trusted Execution Environments (TEEs) in the context of blockchains. This list includes articles, research papers, tweet threads, code repositories, videos, and more.

## What are TEEs?

A Trusted Execution Environment (TEE) is a secure, isolated area within a device or network designed to safeguard sensitive data during storage, processing, and execution. TEEs provide a protected space where programs can run with confidentiality and integrity, even if the broader system is compromised, ensuring tamper-resistant computation.

In addition to this security, TEEs offer attestation capabilities that provide enhanced trust guarantees. Attestation is a cryptographic proof that allows a TEE to verify to a remote party that a program is running (or has run) without any interference. This mechanism reinforces trust in the TEE by proving that specific operations have been executed without tampering, offering third-party verification of computational correctness.

## Table of Contents

1. [Cloud Providers](#cloud-providers)
   - [Google Cloud Confidential Compute](#google-cloud-confidential-compute)
   - [Microsoft Azure Confidential Computing](#microsoft-azure-confidential-computing)
   - [Amazon AWS Nitro](#amazon-aws-nitro)
2. [Hardware](#hardware)
   - [AMD](#amd)
   - [Intel](#intel)
   - [NVIDIA](#nvidia)
   - [ARM](#arm)
3. [Use Cases](#use-cases)
   - [Block Building](#block-building)
   - [Bridging](#bridging)
   - [Asset Management](#asset-management)
   - [General Compute](#general-compute)
   - [Privacy](#privacy)
   - [Rollups](#rollups)
4. [Repositories](#repositories)
   - [General](#general)
   - [Rust](#rust)
   - [Go](#go)
   - [C++](#cpp)
   - [C](#c)
   - [Python](#python)
5. [Research Papers](#research-papers)
6. [Articles](#articles)
7. [Videos](#videos)
8. [Tweet Threads](#tweet-threads)

## Cloud Providers

### Google Cloud Confidential Compute

- [Confidential Accelerator for AI workloads](https://cloud.google.com/blog/products/identity-security/expanding-confidential-computing-for-ai-workloads-next24) - Supports Intel TDX with Intel AMX, and NVIDIA H100 GPUs.
- [Confidential VMs](https://cloud.google.com/blog/products/identity-security/introducing-google-cloud-confidential-computing-with-confidential-vms) - Supports AMD SEV, AMD SEV-SNP, and Intel TDX.
- [Confidential Space](https://cloud.google.com/docs/security/confidential-space) - Supports trust model where the workload author, workload operator, and resource owners are separate, mutually distrusting parties.
- [Confidential VM attestation](https://cloud.google.com/confidential-computing/confidential-vm/docs/attestation) - Attestation support for AMD SEV (vTPM), AMD SEV-SNP (vTPM and TSM), and Intel TDX (vTPM and TSM).

### Microsoft Azure Confidential Computing

- [Azure Confidential VM](https://learn.microsoft.com/en-us/azure/confidential-computing/confidential-vm-overview)

### Amazon AWS Nitro

- [Nitro](https://aws.amazon.com/ec2/nitro/)
- [Nitro Enclaves](https://aws.amazon.com/ec2/nitro/nitro-enclaves/)

## Hardware

### AMD

- [Secure Encrypted Virtualization-Trusted I/O (SEV-TIO)](https://www.amd.com/content/dam/amd/en/documents/developer/sev-tio-whitepaper.pdf) - Improved I/O performance and security in AMD SEV-SNP guests
- [Secure Encrypted Virtualization-Secure Nested Paging (SEV-SNP)](https://www.amd.com/content/dam/amd/en/documents/epyc-business-docs/white-papers/SEV-SNP-strengthening-vm-isolation-with-integrity-protection-and-more.pdf) - Expands on SEV, adds memory integrity protection to help prevent malicious hypervisor-based attacks
- [Secure Encrypted Virtualization (SEV)](https://www.amd.com/en/developer/sev.html) - Hardware-based memory encryption through the AMD Secure Processor

### Intel

- [Advanced Matrix Extensions (AMX)](https://www.intel.com/content/www/us/en/products/docs/accelerator-engines/advanced-matrix-extensions/overview.html) - Accelerator to improve the performance of deep-learning training and inference on the CPU
- [Trust Domain Extensions (TDX)](https://www.intel.com/content/www/us/en/developer/tools/trust-domain-extensions/overview.html?wapkw=TDX) - Latest Hardware-based TEE architecture from Intel
- [Software Guard Extensions (SGX)](https://www.intel.com/content/www/us/en/products/docs/accelerator-engines/software-guard-extensions.html) - Protects data actively being used in the processor and memory by creating a TEE

### NVIDIA

- [H100 TensorCore GPU](https://www.nvidia.com/en-us/data-center/h100/?ncid=so-link-915436-vt04#cid=hpc09_so-link_en-us) - Hardware-based trusted execution environment with NVIDIA Hopper and NVIDIA Blackwell architecture support
- [Hopper Architecture](https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/) - Accelerated computing platform for AI
- [Blackwell Architecture](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/) - Latest HW generation with accelerated computing and generative AI optimizations

### ARM

- [Confidential Compute Architecture (CCA)](https://www.arm.com/architecture/security-features/arm-confidential-compute-architecture) - Under development. Key component of the Armv9-A architecture
- [TrustZone](https://www.arm.com/technologies/trustzone-for-cortex-m#:~:text=Arm%20TrustZone%20technology%20is%20used,to%20as%20the%20secure%20monitor.) - Isolates critical security firmware, assets and private information for Armv8-M based devices

## Use Cases

### Block Building

- [The Future of MEV is SUAVE](https://writings.flashbots.net/the-future-of-mev-is-suave)
- [Block Building inside SGX](https://writings.flashbots.net/block-building-inside-sgx)
- [Running Geth within SGX: Our Experience, Learnings and Code](https://writings.flashbots.net/geth-inside-sgx)
- [SGX-Based Backrunning and Covert Channels](https://writings.flashbots.net/backrunning-private-txs-MPC#sgx-based-backrunning-and-covert-channels)
- [MEV-SGX - A sealed bid MEV auction design](https://ethresear.ch/t/mev-sgx-a-sealed-bid-mev-auction-design/9677)

### Bridging

- Avalanche Bridge - [Website](https://medium.com/avalancheavax/avalanche-bridge-secure-cross-chain-asset-transfers-using-intel-sgx-b04f5a4c7ad1), [ava-labs GitHub](https://github.com/ava-labs)

### Asset Management

- Turnkey - [Website](https://www.turnkey.com), [tkhq GitHub](https://github.com/tkhq)
- Fireblocks - [Website](https://developers.fireblocks.com/docs/what-is-fireblocks#layer-2-secure-enclave), [fireblocks GitHub](https://github.com/fireblocks)
- Cycles Money - [Website](https://cycles.money)
- Solana Saga Seed Vault - [Website](https://solanamobile.com), [solana-mobile GitHub](https://github.com/solana-mobile)

### General Compute

- Marlin Protocol - [Website](https://www.marlin.org/), [marlinprotocol GitHub](https://github.com/marlinprotocol)
- Phala Network - [Website](https://phala.network/), [Phala-Network GitHub](https://github.com/Phala-Network)
- Automata Network - [Website](https://ata.network/), [automata-network GitHub](https://github.com/automata-network)

### Privacy

- Oasis Protocol - [Website](https://oasisprotocol.org), [oasisprotocol GitHub](https://github.com/oasisprotocol)
- Secret Network - [Website](https://scrt.network), [scrtlabs GitHub](https://github.com/scrtlabs)
- Enclave Markets - [Website](https://www.enclave.market)

### Rollups

- Taiko - [Website](https://taiko.xyz/), [taikoxyz GitHub](https://github.com/taikoxyz)

## Repositories

### General

- [sbellem/qtee](https://github.com/sbellem/qtee) - Exploring the physical limits of trusted hardware in the classical and quantum settings to achieve security through physics.

### Rust

- [marlinprotocol/oyster-serverless](https://github.com/marlinprotocol/oyster-serverless) - Oyster Serverless is a cutting-edge, high-performance serverless computing platform designed to securely execute JavaScript (JS) and WebAssembly (WASM) code in a highly controlled environment.
- [Phala-Network/phala-blockchain](https://github.com/Phala-Network/phala-blockchain) - The Phala Network Blockchain, pRuntime and the bridge.
- [kata-containers/kata-containers](https://github.com/kata-containers/kata-containers) - Kata Containers is an open source project and community working to build a standard implementation of lightweight Virtual Machines (VMs) that feel and perform like containers, but provide the workload isolation and security advantages of VMs.
- [taikoxyz/raiko](https://github.com/taikoxyz/raiko) - Multi-proofs for Taiko. SNARKS, STARKS and Trusted Execution Enclave.
- [confidential-containers/guest-components](https://github.com/confidential-containers/guest-components) - Confidential Containers Guest Tools and Components
- [kinvolk/azure-cvm-tooling](https://github.com/kinvolk/azure-cvm-tooling) - Libraries and tools for Confidential Computing on Azure
- [HyperEnclave/hyperenclave](https://github.com/HyperEnclave/hyperenclave) - An Open and Cross-platform Trusted Execution Environment.
- [mobilecoinfoundation/mobilecoin](https://github.com/mobilecoinfoundation/mobilecoin) - Private payments for mobile devices
- [integritee-network/worker](https://github.com/integritee-network/worker) - Integritee off-chain worker and sidechain validateer
- [capsule-corp-ternoa/ternoa-node](https://github.com/capsule-corp-ternoa/ternoa-node) - Ternoa's Node Implementation
- [automata-network/automata](https://github.com/automata-network/automata) - Automata Network is a modular attestation layer that extends machine trust to Ethereum with TEE Coprocessors.
- [apache/incubator-teaclave-sgx-sdk](https://github.com/apache/incubator-teaclave-sgx-sdk) - Apache Teaclave (incubating) SGX SDK helps developers to write Intel SGX applications in the Rust programming language, and also known as Rust SGX SDK.
- [apache/incubator-teaclave](https://github.com/apache/incubator-teaclave) - Apache Teaclave (incubating) is an open source universal secure computing platform, making computation on privacy-sensitive data safe and simple.
- [scrtlabs/incubator-teaclave-sgx-sdk](https://github.com/scrtlabs/incubator-teaclave-sgx-sdk) - Rust SGX SDK provides the ability to write Intel SGX applications in Rust Programming Language. Fork of `apache/incubator-teaclave-sgx-sdk`.

### Go

- [google/go-tpm-tools](https://github.com/google/go-tpm-tools) - Go packages built on go-tpm providing a high-level API for using TPMs
- [google/go-sev-guest](https://github.com/google/go-sev-guest) - go-sev-guest offers a library to wrap the /dev/sev-guest device in Linux, as well as a library for attestation verification of fundamental components of an attestation report.
- [google/go-tdx-guest](https://github.com/google/go-tdx-guest) - go-tdx-guest offers a library to wrap the /dev/tdx-guest device in Linux, as well as a library for attestation verification of fundamental components of an attestation quote.
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

- [iisec-suzaki/optee-ra](https://github.com/iisec-suzaki/optee-ra) - OP-TEE Remote Attestation
- [pietroborrello/CustomProcessingUnit](https://github.com/pietroborrello/CustomProcessingUnit) - The first analysis framework for CPU microcode
- [openenclave/openenclave](https://github.com/openenclave/openenclave) - SDK for developing enclaves
- [deislabs/mystikos](https://github.com/deislabs/mystikos) - Tools and runtime for launching unmodified container images in Trusted Execution Environments
- [openenclave/openenclave](https://github.com/openenclave/openenclave) - SDK for developing enclaves
- [mofanv/PPFL](https://github.com/mofanv/PPFL) - Privacy-preserving Federated Learning with Trusted Execution Environments
- [inclavare-containers/inclavare-containers](https://github.com/inclavare-containers/inclavare-containers) - A novel container runtime, aka confidential container, for cloud-native confidential computing and enclave runtime ecosystem.

### Python

- [ethernity-cloud/mvp-pox-node](https://github.com/ethernity-cloud/mvp-pox-node) - Ethernity Cloud Node

### TS

- [tkhq/sdk](https://github.com/tkhq/sdk) - Turnkey TypeScript SDK

## Research Papers

- J. Zhu, H. Yin, P. Deng, and S. Zhou, "Confidential Computing on nVIDIA H100 GPU: A Performance Benchmark Study", 2024 - [arXiv](https://arxiv.org/abs/2409.03992)
- A. Sunny, N, Shrivastava, S. and R. Sarangi, "SecScale: A Scalable and Secure Trusted Execution Environment for Servers", 2024 - [arXiv](https://arxiv.org/abs/2407.13572)
- H. Eichner, D. Ramage, K. Bonawitz, D. Huba et. al., "Confidential Federated Computations", 2024 - [arXiv](https://arxiv.org/abs/2404.10764)
- X. Zhang, K. Qin, S. Qu, T. Wang, C. Zhang, and D. Gu "Teamwork Makes TEE Work: Open and Resilient Remote Attestation on Decentralized Trust", 2024 - [arXiv](https://arxiv.org/abs/2402.08908)
- Y. Xian, L. Zhou, J. Jiang, B. Wang, H. Huo, and P. Liu, "A Distributed Efficient Blockchain Oracle Scheme for Internet of Things", 2023 - [arXiv](https://arxiv.org/abs/2310.00254)
- A. P. Kalapaaking, I. Khalil, M. S. Rahman, M. Atiquzzaman, X. Yi, and M. Almashor, "Blockchain-based Federated Learning with Secure Aggregation in Trusted Execution Environment for Internet-of-Things", 2023 - [arXiv](https://arxiv.org/abs/2304.12889)
- M. Schneider, R.J. Masti, S. Shinde, S. Capkun, and R. Perez, "SoK: Hardware-supported Trusted Execution Environments", 2022 - [arXiv](https://arxiv.org/abs/2205.12742)
- R. Li, Q. Wang, Q. Wang, D. Galindo, and M. Ryan, "SoK: TEE-assisted Confidential Smart Contract", 2022 - [arXiv](https://arxiv.org/abs/2203.08548)
- E. Puschner, T. Moos, S. Becker, C. Kison, A. Moradi, C. Paar, "Red Team vs. Blue Team: A Real-World Hardware Trojan Detection Case Study Across Four Modern CMOS Technology Generations", 2022 - [Cryptology ePrint Archive](https://eprint.iacr.org/2022/1720)
- R. Karanjai, L. Xu, L. Chen, F. Zhang, Z. Gao, and W. Shi, "Lessons Learned from Blockchain Applications of Trusted Execution Environments and Implications for Future Research", 2022 - [arXiv](https://arxiv.org/abs/2203.12724)
- C. Liu, H. Guo, M. Xu, S. Wang, D. Yu, J. Yu, and X. Cheng, "Extending On-chain Trust to Off-chain -- Trustworthy Blockchain Data Collection using Trusted Execution Environment (TEE)", 2021 - [arXiv](https://arxiv.org/abs/2106.15934)
- D. Natarajan, A. Loveless, W. Dai, and R. Dreslinski, “CHEX-MIX: Combining Homomorphic Encryption with Trusted Execution Environments for Two-party Oblivious Inference in the Cloud”, 2021. - [Cryptology ePrint Archive](https://eprint.iacr.org/2021/1603)
- Z. Bao, Q. Wang, W. Shi, L. Wang, H. Lei, and B. Chen, "When Blockchain Meets SGX: An Overview, Challenges, and Open Issues", 2020 - [IEEE](https://ieeexplore.ieee.org/document/9197584)
- A. Nilsson, P. N. Bideh, and J. Brorsson, “A Survey of Published Attacks on Intel SGX”, 2020. - [arXiv](http://arxiv.org/abs/2006.13598)
- K. Murdock, D. Oswald, F. D. Garcia, J. Van Bulck, D. Gruss, and F. Piessens, “Plundervolt: Software-based Fault Injection Attacks against Intel SGX”, 2020. - [IEEE](https://ieeexplore.ieee.org/document/9152636)
- R. Cheng, F. Zhang, J. Kos, W. He, N. Hynes, N. Johnson, A. Juels, and A. Miller, "Ekiden: A Platform for Confidentiality-Preserving, Trustworthy, and Performant Smart Contracts", 2019 - [IEEE](https://ieeexplore.ieee.org/document/8806762)
- G. Kaptchuk, I. Miers, and M. Green, "Giving State to the Stateless: Augmenting Trustworthy Computation with Ledgers" , 2017 - [Cryptology ePrint Archive](https://eprint.iacr.org/2017/201)
- J. Lind, O. Naor, I. Eyal, F. Kelbert, P. Pietzuch, and E. Gun Sirer, "Teechain: A Secure Payment Network with Asynchronous Blockchain Access", 2017. - [arXiv](https://arxiv.org/abs/1707.05454)

## Articles

- [A few notes on AWS Nitro Enclaves: Attack surface - Trail of Bits Blog](https://blog.trailofbits.com/2024/09/24/notes-on-aws-nitro-enclaves-attack-surface/)
- [Early Thoughts on Decentralized Root-of-Trust - Flashbots Collective](https://collective.flashbots.net/t/early-thoughts-on-decentralized-root-of-trust/3868)
- [Drawbacks In FHE Blockchain And How TEE Can Help It - Flashbots Collective](https://collective.flashbots.net/t/drawbacks-in-fhe-blockchain-and-how-tee-can-help-it/3642)
- [Building Secure Ethereum Blocks on Minimal Intel TDX Confidential VMs - Flashbots Collective](https://collective.flashbots.net/t/building-secure-ethereum-blocks-on-minimal-intel-tdx-confidential-vms/3795)
- [TDX Security For BOB Searchers, Flashbots](https://flashbots.notion.site/TDX-Security-For-BOB-Searchers-aedb060eb75b48a2a5de0e2131c9c7ef)
- [Chapter 3 - Verifiable Off-chain Compute: Enabling an Instagram-like experience for Web3 - Florin Digital](https://florindigital.substack.com/p/chapter-3-verifiable-off-chain-compute)
- [Sirrah: Speedrunning a TEE Coprocessor](https://writings.flashbots.net/suave-tee-coprocessor)
- [Demystifying SGX — Part 1 - Obscuro Labs](https://medium.com/obscuro-labs/intel-sgx-demystified-757a242682a3)
- [Blockchain Privacy and Security in Data Computation](https://www.zkon.xyz/blog/blockchain-privacy-mpc-zk-tee-explained)
- [Trustless Execution Environments - David Atterman](https://omnida.substack.com/p/trustless-execution-environments?r=nvn5c&utm_campaign=post&utm_medium=web&triedRedirect=true)
- [4 Ways to Compare Trusted Execution Environments and Zero-Knowledge Proofs](https://oasisprotocol.org/blog/comparing-zkp-tee-privacy)
- [What is a Trusted Execution Environment (TEE)? - Halborn](https://www.halborn.com/blog/post/what-is-a-trusted-execution-environment-tee)
- [How Secret Network Uses SGX](https://docs.scrt.network/secret-network-documentation/overview-ecosystem-and-technology/techstack/privacy-technology/intel-sgx/overview)
- [Blockchain × TEE: Why Various Forefront Projects are Adopting TEE - TOKI](https://medium.com/@tokifinance/blockchain-projects-adapting-tee-bed9550db9c5)
- [Why trusted execution environments will be integral to proof-of-stake blockchains](https://venturebeat.com/datadecisionmakers/why-trusted-execution-environments-will-be-integral-to-proof-of-stake-blockchains/)
- [TEE-based Smart Contracts and Sealing Pitfalls](https://medium.com/initc3org/tee-based-smart-contracts-and-sealing-pitfalls-eccd5d751329)
- [Trusted Execution Environments and the Polkadot Ecosystem](https://polkadot.network/blog/trusted-execution-environments-and-the-polkadot-ecosystem)
- [Blockchains in Trusted Execution Environments (TEEs)](https://medium.com/@nadeem.bhati/blockchains-in-trusted-execution-environments-tees-9343b6c3f9e8)
- [Intel SGX and Blockchain: The iExec End-to-End Trusted Execution Solution](https://medium.com/iex-ec/iexec-end-to-end-sgx-solution-fee1e63297b2)
- [Blockchains + TEEs Day 1 Summary](https://decentralizedthoughts.github.io/2023-04-09-blockchainsplustees-day1-summary/)
- [Blockchains + TEEs Day 2 Summary](https://decentralizedthoughts.github.io/2023-04-17-blockchainsplustees-day2-summary/)
- [Intel SGX Explained](https://css.csail.mit.edu/6.858/2020/readings/costan-sgx.pdf)

## Videos

- [Phala Network: 'The Magic of TEEs' - Online Workshop on TEE Basics](https://www.youtube.com/watch?v=Rpv4ZNOcNsM)
- [How to Win Friends and TEE-fluence People - Ethan Buchman, Modular Summit 2024](https://youtu.be/XwKIt5XYyqw)
- [DEVMOS 2024: Dylan Kawalec (Osmosis), 'Building Decentralized Frontends', Modular Summit 2024](https://youtu.be/o1TY6sjMOek)
- [The TEE Stack - Andrew Miller, Modular Summit 2024](https://youtu.be/9AwlMB8TF4o)
- [What apps are unlocked by the TEE stack - Xinyuan Sun, Modular Summit 2024](https://x.com/modular_summit/status/1814653436090327161)
- [Parallelized Confidential Computing - Yannik Schrade, Fil Dev Summit 2024](https://youtu.be/k0Uxl71Lj_g)
- [TEE for Blockchain Applications - Ari Juels, a16z crypto 2023](https://youtu.be/Xq7oWtiwWII)
- [Private Smart Contracts are Worth the Price of the SGX - Andrew Miller, ETHDenver 2023](https://youtu.be/L0bp6V1pn0s)
- [Protected Order Flow for Fair Transaction-Ordering in a Profit-Seeking World - Kushal Babel, MEV-SBC 2023](https://youtu.be/v1TkocRScJg)
- [Blockchains + TEEs 2023: Day 1 - Kartik Nayan, Ittai Abraham, Aniket Kate](https://youtu.be/9-nhNQO5_Js)
- [Blockchains + TEEs 2023: Day 2 - Kartik Nayan, Ittai Abraham, Aniket Kate](https://youtu.be/zIU3gFTb2PM)
- [SGX Panel 2023: Andrew Miller, Jonathan Passerat Palmbach, Phil Daian, Justin Drake](https://youtu.be/vokDXJmPCSI)
- [Enabling Cross Chain Transfers Using SGX - Michael Kaplan, Avalanche Summit 2022](https://youtu.be/f2bU55ngO_c)
- [Trusted Execution Environments Meet the Blockchain - Ittay Eyal, Simons Institute 2019](https://youtu.be/J-8RdvvpUzM)

## Tweet threads

- [@\_markel\_\_\_, Extraction of Intel SGX Fuse Key0](https://x.com/_markel___/status/1828112469010596347)
- [@PratyushRT, Breakdown of the Intel SGX (TEE) breach](https://x.com/pratyushrt/status/1828183761055330373?s=46)
- [@buchmanster, TEE, ZK, FHE and MPC](https://x.com/buchmanster/status/1816084691784720887)
- [@buchmanster, How you win friends and TEE-fluence people - Chapter 2](https://x.com/buchmanster/status/1816443327241490662)
- [@DistributedMarz, Flashwares Live Session](https://x.com/DistributedMarz/status/1805640541360550110)
