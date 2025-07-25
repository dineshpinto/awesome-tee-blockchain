# Awesome TEE Blockchain [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of resources for learning about Trusted Execution Environments (TEEs) and their applications in the blockchain space.

_Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md)._

- [Getting Started](#getting-started)
- [Articles](#articles)
- [Research Papers](#research-papers)
- [Hardware Platforms](#hardware-platforms)
- [Cloud Solutions](#cloud-solutions)
- [Blockchain Applications & Use Cases](#blockchain-applications--use-cases)
- [Code Repositories](#code-repositories)
  - [Rust](#rust)
  - [Go](#go)
  - [CPP](#cpp)
  - [C](#c)
  - [Others](#others)
- [Social Media & Community](#social-media--community)
- [Additional Resources](#additional-resources)

## Getting Started

_Articles, talks and presentations to help you get started with TEEs._

- **Articles**
  - [Verifiable Off-chain Compute: Enabling an Instagram-like experience for Web3 - Florin Digital](https://florindigital.substack.com/p/chapter-3-verifiable-off-chain-compute)
  - [What is a Trusted Execution Environment (TEE)? - Halborn](https://www.halborn.com/blog/post/what-is-a-trusted-execution-environment-tee)
  - [Trustless Execution Environments - David Atterman](https://omnida.substack.com/p/trustless-execution-environments?r=nvn5c&utm_campaign=post&utm_medium=web&triedRedirect=true)
  - [Why trusted execution environments will be integral to proof-of-stake blockchains](https://venturebeat.com/datadecisionmakers/why-trusted-execution-environments-will-be-integral-to-proof-of-stake-blockchains/)
  - [Blockchain Privacy and Security in Data Computation](https://www.zkon.xyz/blog/blockchain-privacy-mpc-zk-tee-explained)
  - [Blockchain x TEE: Why Various Forefront Projects are Adopting TEE - TOKI](https://medium.com/@tokifinance/blockchain-projects-adapting-tee-bed9550db9c5)
  - [4 Ways to Compare Trusted Execution Environments and Zero-Knowledge Proofs](https://oasisprotocol.org/blog/comparing-zkp-tee-privacy)
  - [Blockchains in Trusted Execution Environments (TEEs)](https://medium.com/@nadeem.bhati/blockchains-in-trusted-execution-environments-tees-9343b6c3f9e8)
- **Conference Talks**
  - [How to Win Friends and TEE-fluence People - Ethan Buchman, Modular Summit 2024](https://youtu.be/XwKIt5XYyqw)
  - [The TEE Stack - Andrew Miller, Modular Summit 2024](https://youtu.be/9AwlMB8TF4o)
  - [Private Smart Contracts are Worth the Price of the SGX - Andrew Miller, ETHDenver 2023](https://youtu.be/L0bp6V1pn0s)
  - [Protected Order Flow for Fair Transaction-Ordering in a Profit-Seeking World - Kushal Babel, MEV-SBC 2023](https://youtu.be/v1TkocRScJg)
  - [Enabling Cross Chain Transfers Using SGX - Michael Kaplan, Avalanche Summit 2022](https://youtu.be/f2bU55ngO_c)
  - [Trusted Execution Environments Meet the Blockchain - Ittay Eyal, Simons Institute 2019](https://youtu.be/J-8RdvvpUzM)
- **Technical Presentations**
  - [DEVMOS 2024: Dylan Kawalec (Osmosis), 'Building Decentralized Frontends', Modular Summit 2024](https://youtu.be/o1TY6sjMOek)
  - [What apps are unlocked by the TEE stack - Xinyuan Sun, Modular Summit 2024](https://x.com/modular_summit/status/1814653436090327161)
  - [Parallelized Confidential Computing - Yannik Schrade, Fil Dev Summit 2024](https://youtu.be/k0Uxl71Lj_g)
  - [TEE for Blockchain Applications - Ari Juels, a16z crypto 2023](https://youtu.be/Xq7oWtiwWII)
  - [SGX Panel 2023: Andrew Miller, Jonathan Passerat Palmbach, Phil Daian, Justin Drake](https://youtu.be/vokDXJmPCSI)
- **Workshops & Tutorials**
  - [Phala Network: 'The Magic of TEEs' - Online Workshop on TEE Basics](https://www.youtube.com/watch?v=Rpv4ZNOcNsM)
  - [Blockchains + TEEs 2023: Day 1 - Kartik Nayan, Ittai Abraham, Aniket Kate](https://youtu.be/9-nhNQO5_Js)
  - [Blockchains + TEEs 2023: Day 2 - Kartik Nayan, Ittai Abraham, Aniket Kate](https://youtu.be/zIU3gFTb2PM)
  - [An intro to SGX & Enclave-based API with Kevin Yu | ETHDenver Privacy Workshop](https://www.youtube.com/watch?v=N_e-b1XL4vM)
  - [TEE-based Web2 User Data Attestations](https://vimeo.com/923289638?share=copy)

### Articles

- **Advanced**
  - [Proprietary binary provisioning within TEEs - fnerdman](https://collective.flashbots.net/t/proprietary-binary-provisioning-within-tees/3394)
  - [We call this kernel saunters: How Apple rearranged its XNU core with exclaves - The Register](https://www.theregister.com/2025/03/08/kernel_sanders_apple_rearranges_xnu/)
  - [Building Secure Ethereum Blocks on Minimal Intel TDX Confidential VMs - Flashbots Collective](https://collective.flashbots.net/t/building-secure-ethereum-blocks-on-minimal-intel-tdx-confidential-vms/3795)
  - [TDX Security For BOB Searchers, Flashbots](https://flashbots.notion.site/TDX-Security-For-BOB-Searchers-aedb060eb75b48a2a5de0e2131c9c7ef)
  - [Sirrah: Speedrunning a TEE Coprocessor](https://writings.flashbots.net/suave-tee-coprocessor)
  - [Nix + Bazel: Fully reproducible, incremental builds](https://www.tweag.io/blog/2018-03-15-bazel-nix/)
  - [Early Thoughts on Decentralized Root-of-Trust - Flashbots Collective](https://collective.flashbots.net/t/early-thoughts-on-decentralized-root-of-trust/3868)
  - [Drawbacks In FHE Blockchain And How TEE Can Help It - Flashbots Collective](https://collective.flashbots.net/t/drawbacks-in-fhe-blockchain-and-how-tee-can-help-it/3642)
  - [How Secret Network Uses SGX](https://docs.scrt.network/secret-network-documentation/overview-ecosystem-and-technology/techstack/privacy-technology/intel-sgx/overview)
  - [Trusted Execution Environments and the Polkadot Ecosystem](https://polkadot.network/blog/trusted-execution-environments-and-the-polkadot-ecosystem)
  - [Intel SGX and Blockchain: The iExec End-to-End Trusted Execution Solution](https://medium.com/iex-ec/iexec-end-to-end-sgx-solution-fee1e63297b2)
  - [Blockchains + TEEs Day 1 Summary](https://decentralizedthoughts.github.io/2023-04-09-blockchainsplustees-day1-summary/)
  - [Blockchains + TEEs Day 2 Summary](https://decentralizedthoughts.github.io/2023-04-17-blockchainsplustees-day2-summary/)
  - [Intel SGX Explained](https://css.csail.mit.edu/6.858/2020/readings/costan-sgx.pdf)
  - [Demystifying SGX — Part 1 - Obscuro Labs](https://medium.com/obscuro-labs/intel-sgx-demystified-757a242682a3)
- **Security**
  - [A Survey of Published Attacks on Intel SGX - Nilsson et al. (2020)](https://arxiv.org/abs/2006.13598)
  - [Plundervolt: Software-based Fault Injection Attacks against Intel SGX - Murdock et al. (2020)](https://ieeexplore.ieee.org/document/9152636)
  - [Securing TEE Apps: A Developer's Guide - Bedlam Research](https://www.bedlamresear.ch/posts/securing-tee-apps)
  - [TEE-based Smart Contracts and Sealing Pitfalls - IC3](https://medium.com/initc3org/tee-based-smart-contracts-and-sealing-pitfalls-eccd5d751329)
  - [A few notes on AWS Nitro Enclaves: Attack surface - Trail of Bits Blog](https://blog.trailofbits.com/2024/09/24/notes-on-aws-nitro-enclaves-attack-surface/)

## Research Papers

_Key research works covering different aspects of TEEs._

- **2025**
  - [NVIDIA GPU Confidential Computing Demystified](https://arxiv.org/abs/2507.02770) - Z. Gu, E. Valdez, S. Ahmed, J. J. Stephen, M. Le, H. Jamjoom, S. Zhao, and Zhiqiang Lin, arXiv, 2025.
  - [Performance of Confidential Computing GPUs](https://www.arxiv.org/abs/2505.16501) - A. M. Ibarra, J. J. Stephen, A. G. Vidal, K. R. Jayaram, and A. F. Gomez, arXiv, 2025.
  - [TeeRollup: Efficient Rollup Design Using Heterogeneous TEE](https://arxiv.org/abs/2409.14647v2) - X. Wen, Q. Feng, H. Lyu, J. Niu, Y. Zhang, and C. Feng, arXiv, 2025.
- **2024**
  - [Towards Validation of TLS 1.3 Formal Model and Vulnerabilities in Intel's RA‑TLS Protocol](https://ieeexplore.ieee.org/document/10752524/) - M. U. Sardar, A. Niemi, H. Tschofenig, and T. Fossati, IEEE, 2024.
  - [Confidential Computing on nVIDIA H100 GPU: A Performance Benchmark Study](https://arxiv.org/abs/2409.03992) - J. Zhu, H. Yin, P. Deng, and S. Zhou, arXiv, 2024.
  - [SecScale: A Scalable and Secure Trusted Execution Environment for Servers](https://arxiv.org/abs/2407.13572) - A. Sunny, N. Shrivastava, S., and R. Sarangi, arXiv, 2024.
  - [Confidential Federated Computations](https://arxiv.org/abs/2404.10764) - H. Eichner, D. Ramage, K. Bonawitz, D. Huba, et al., arXiv, 2024.
  - [Teamwork Makes TEE Work: Open and Resilient Remote Attestation on Decentralized Trust](https://arxiv.org/abs/2402.08908) - X. Zhang, K. Qin, S. Qu, T. Wang, C. Zhang, and D. Gu, arXiv, 2024.
- **2023**
  - [Intel TDX Demystified: A Top‑Down Approach](https://arxiv.org/abs/2303.15540) - P. Chen, W. Ozga, E. Valdez, S. Ahmed, Z. Gu, H. Jamjoom, U. Franke, and J. Bottomley, arXiv, 2023.
  - [A Distributed Efficient Blockchain Oracle Scheme for Internet of Things](https://arxiv.org/abs/2310.00254) - Y. Xian, L. Zhou, J. Jiang, B. Wang, H. Huo, and P. Liu, arXiv, 2023.
  - [Blockchain‑based Federated Learning with Secure Aggregation in Trusted Execution Environment for Internet‑of‑Things](https://arxiv.org/abs/2304.12889) - A. P. Kalapaaking, I. Khalil, M. S. Rahman, M. Atiquzzaman, X. Yi, and M. Almashor, arXiv, 2023.
- **2022**
  - [SoK: Hardware‑supported Trusted Execution Environments](https://arxiv.org/abs/2205.12742) - M. Schneider, R. J. Masti, S. Shinde, S. Capkun, and R. Perez, arXiv, 2022.
  - [SoK: TEE‑assisted Confidential Smart Contract](https://arxiv.org/abs/2203.08548) - R. Li, Q. Wang, Q. Wang, D. Galindo, and M. Ryan, arXiv, 2022.
  - [Red Team vs. Blue Team: A Real‑World Hardware Trojan Detection Case Study Across Four Modern CMOS Technology Generations](https://eprint.iacr.org/2022/1720) - E. Puschner, T. Moos, S. Becker, C. Kison, A. Moradi, and C. Paar, Cryptology ePrint Archive, 2022.
  - [Lessons Learned from Blockchain Applications of Trusted Execution Environments and Implications for Future Research](https://arxiv.org/abs/2203.12724) - R. Karanjai, L. Xu, L. Chen, F. Zhang, Z. Gao, and W. Shi, arXiv, 2022.
- **2021**
  - [Extending On‑chain Trust to Off‑chain - Trustworthy Blockchain Data Collection using Trusted Execution Environment (TEE)](https://arxiv.org/abs/2106.15934) - C. Liu, H. Guo, M. Xu, S. Wang, D. Yu, J. Yu, and X. Cheng, arXiv, 2021.
  - [CHEX‑MIX: Combining Homomorphic Encryption with Trusted Execution Environments for Two‑party Oblivious Inference in the Cloud](https://eprint.iacr.org/2021/1603) - D. Natarajan, A. Loveless, W. Dai, and R. Dreslinski, Cryptology ePrint Archive, 2021.
- **Pre‑2020**
  - [When Blockchain Meets SGX: An Overview, Challenges, and Open Issues](https://ieeexplore.ieee.org/document/9197584) - Z. Bao, Q. Wang, W. Shi, L. Wang, H. Lei, and B. Chen, IEEE, 2020.
  - [Ekiden: A Platform for Confidentiality‑Preserving, Trustworthy, and Performant Smart Contracts](https://ieeexplore.ieee.org/document/8806762) - R. Cheng, F. Zhang, J. Kos, W. He, N. Hynes, N. Johnson, A. Juels, and A. Miller, IEEE, 2019.
  - [Giving State to the Stateless: Augmenting Trustworthy Computation with Ledgers](https://eprint.iacr.org/2017/201) - G. Kaptchuk, I. Miers, and M. Green, Cryptology ePrint Archive, 2017.
  - [Teechain: A Secure Payment Network with Asynchronous Blockchain Access](https://arxiv.org/abs/1707.05454) - J. Lind, O. Naor, I. Eyal, F. Kelbert, P. Pietzuch, and E. Gun Sirer, arXiv, 2017.

## Hardware Platforms

_The underlying silicon providing TEE capabilities._

- **Intel**
  - [Advanced Matrix Extensions (AMX)](https://www.intel.com/content/www/us/en/products/docs/accelerator-engines/advanced-matrix-extensions/overview.html) - Accelerator to improve the performance of deep-learning training and inference on the CPU.
  - [Trust Domain Extensions (TDX)](https://www.intel.com/content/www/us/en/developer/tools/trust-domain-extensions/overview.html?wapkw=TDX) - Latest Hardware-based TEE architecture from Intel.
  - [Software Guard Extensions (SGX)](https://www.intel.com/content/www/us/en/products/docs/accelerator-engines/software-guard-extensions.html) - Protects data actively being used in the processor and memory by creating a TEE.
- **AMD**
  - [Secure Encrypted Virtualization-Trusted I/O (SEV-TIO)](https://www.amd.com/content/dam/amd/en/documents/developer/sev-tio-whitepaper.pdf) - Improved I/O performance and security in AMD SEV-SNP guests.
  - [Secure Encrypted Virtualization-Secure Nested Paging (SEV-SNP)](https://www.amd.com/content/dam/amd/en/documents/epyc-business-docs/white-papers/SEV-SNP-strengthening-vm-isolation-with-integrity-protection-and-more.pdf) - Expands on SEV, adds memory integrity protection to help prevent malicious hypervisor-based attacks.
  - [Secure Encrypted Virtualization (SEV)](https://www.amd.com/en/developer/sev.html) - Hardware-based memory encryption through the AMD Secure Processor.
- **NVIDIA**
  - [H100 TensorCore GPU](https://www.nvidia.com/en-us/data-center/h100/?ncid=so-link-915436-vt04#cid=hpc09_so-link_en-us) - Hardware-based trusted execution environment with NVIDIA Hopper and NVIDIA Blackwell architecture support.
  - [Hopper Architecture](https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/) - Accelerated computing platform for AI.
  - [Blackwell Architecture](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/) - Latest HW generation with accelerated computing and generative AI optimizations.
- **RISC-V**
  - [Keystone](https://keystone-enclave.org) - Open Framework for architecting Trusted Execution Environments built on RISC-V.
- **ARM**
  - [Confidential Compute Architecture (CCA)](https://www.arm.com/architecture/security-features/arm-confidential-compute-architecture) - Under development. Key component of the Armv9-A architecture.
  - [TrustZone](https://www.arm.com/technologies/trustzone-for-cortex-m#:~:text=Arm%20TrustZone%20technology%20is%20used,to%20as%20the%20secure%20monitor.) - Isolates critical security firmware, assets and private information for Armv8-M based devices.
  - [OP-TEE](https://www.trustedfirmware.org/projects/op-tee/) - Companion TEE for a non-secure Linux kernel running on ARM; Cortex-A cores using the TrustZone technology.
- **OpenTitan**
  - [OpenTitan](https://opentitan.org) - Open source project building a reference design and integration guidelines for silicon root of trust (RoT) chips.
  - [lowRISC/opentitan](https://github.com/lowRISC/opentitan) - Open source silicon root of trust.

## Cloud Solutions

_Major cloud providers offering virtual machines or services utilizing TEE hardware._

- **Google Cloud**
  - [Confidential Accelerator for AI workloads](https://cloud.google.com/blog/products/identity-security/expanding-confidential-computing-for-ai-workloads-next24) - Supports Intel TDX with Intel AMX, and NVIDIA H100 GPUs.
  - [Confidential VMs](https://cloud.google.com/blog/products/identity-security/introducing-google-cloud-confidential-computing-with-confidential-vms) - Supports AMD SEV, AMD SEV-SNP, and Intel TDX.
  - [Confidential Space](https://cloud.google.com/docs/security/confidential-space) - Supports trust model where the workload author, workload operator, and resource owners are separate, mutually distrusting parties.
  - [Confidential VM attestation](https://cloud.google.com/confidential-computing/confidential-vm/docs/attestation) - Attestation support for AMD SEV (vTPM), AMD SEV-SNP (vTPM and TSM), and Intel TDX (vTPM and TSM).
- **Amazon AWS**
  - [Nitro](https://aws.amazon.com/ec2/nitro/)
  - [Nitro Enclaves](https://aws.amazon.com/ec2/nitro/nitro-enclaves/)
- **Microsoft Azure**
  - [Azure Confidential VM](https://learn.microsoft.com/en-us/azure/confidential-computing/confidential-vm-overview)
- **Oracle Cloud**
  - [OCI Confidential Compute](https://docs.oracle.com/en-us/iaas/Content/Compute/References/confidential_compute.htm)
- **Alibaba Cloud**
  - [ECS Confidential Computing](https://www.alibabacloud.com/help/en/ecs/user-guide/confidential-computing-capabilities/)

## Blockchain Applications & Use Cases

_Examples of how TEEs are being used or proposed within the blockchain ecosystem._

- **AI**
  - TEN Protocol - [Website](https://ten.xyz), [ten-protocol GitHub](https://github.com/ten-protocol)
  - Aizel Network - [Website](https://aizelnetwork.com), [AizelNetwork GitHub](https://github.com/AizelNetwork)
  - ELIZA in TEE - [TEE plugin for ELIZA (using dstack from Phala)](https://elizaos.github.io/eliza/docs/advanced/eliza-in-tee/)
- **Block Building & MEV Mitigation**
  - Jito BAM - [Website](https://bam.dev)
  - Unichain - [Website](https://www.unichain.org), [Whitepaper](https://docs.unichain.org/whitepaper.pdf)
  - [Block Building inside SGX](https://writings.flashbots.net/block-building-inside-sgx)
  - [Running Geth within SGX: Our Experience, Learnings and Code](https://writings.flashbots.net/geth-inside-sgx)
  - [SGX-Based Backrunning and Covert Channels](https://writings.flashbots.net/backrunning-private-txs-MPC#sgx-based-backrunning-and-covert-channels)
  - [MEV-SGX - A sealed bid MEV auction design](https://ethresear.ch/t/mev-sgx-a-sealed-bid-mev-auction-design/9677)
- **Bridging**
  - Avalanche Bridge - [Website](https://medium.com/avalancheavax/avalanche-bridge-secure-cross-chain-asset-transfers-using-intel-sgx-b04f5a4c7ad1), [ava-labs GitHub](https://github.com/ava-labs)
- **Asset Management & Wallets**
  - Turnkey - [Website](https://www.turnkey.com), [tkhq GitHub](https://github.com/tkhq)
  - Lit Protocol - [Website](https://www.litprotocol.com), [LIT-Protocol GitHub](https://github.com/LIT-Protocol)
  - Fireblocks - [Website](https://developers.fireblocks.com/docs/what-is-fireblocks#layer-2-secure-enclave), [fireblocks GitHub](https://github.com/fireblocks)
  - Cycles Money - [Website](https://cycles.money)
  - Solana Saga Seed Vault - [Website](https://solanamobile.com), [solana-mobile GitHub](https://github.com/solana-mobile)
- **General Off-Chain Compute**
  - Sui Nautilus - [Website](https://sui.io/nautilus), [MystenLabs GitHub](https://github.com/MystenLabs)
  - Marlin Protocol - [Website](https://www.marlin.org/), [marlinprotocol GitHub](https://github.com/marlinprotocol)
  - Phala Network - [Website](https://phala.network/), [Phala-Network GitHub](https://github.com/Phala-Network)
  - Automata Network - [Website](https://ata.network/), [automata-network GitHub](https://github.com/automata-network)
  - Clique Network - [Website](https://www.clique.tech), [automata-network GitHub](https://github.com/automata-network)
- **Privacy & Confidentiality**
  - Oasis Protocol - [Website](https://oasisprotocol.org), [oasisprotocol GitHub](https://github.com/oasisprotocol)
  - Secret Network - [Website](https://scrt.network), [scrtlabs GitHub](https://github.com/scrtlabs)
  - Enclave Markets - [Website](https://www.enclave.market)
- **Rollups & Coprocessors**
  - Taiko - [Website](https://taiko.xyz/), [taikoxyz GitHub](https://github.com/taikoxyz)
  - Unichain - [Website](https://www.unichain.org)

## Code Repositories

_Software related to TEEs in the context of blockchain, libraries, and example implementations._

### Rust

- [MystenLabs/nautilus](https://github.com/MystenLabs/nautilus) - Nautilus: Verifiable offchain computation on Sui.
- [Dstack-TEE/dstack](https://github.com/Dstack-TEE/dstack) - Dstack is a developer friendly and security first SDK to simplify the deployment of arbitrary Docker-based apps into TEE.
- [marlinprotocol/oyster-serverless](https://github.com/marlinprotocol/oyster-serverless) - Oyster Serverless is a cutting-edge, high-performance serverless computing platform designed to securely execute JavaScript (JS) and WebAssembly (WASM) code in a highly controlled environment.
- [Phala-Network/phala-blockchain](https://github.com/Phala-Network/phala-blockchain) - The Phala Network Blockchain, pRuntime and the bridge.
- [kata-containers/kata-containers](https://github.com/kata-containers/kata-containers) - Kata Containers is an open source project and community working to build a standard implementation of lightweight Virtual Machines (VMs) that feel and perform like containers, but provide the workload isolation and security advantages of VMs.
- [taikoxyz/raiko](https://github.com/taikoxyz/raiko) - Multi-proofs for Taiko. SNARKS, STARKS and Trusted Execution Enclave.
- [enarx/drawbridge](https://github.com/enarx/drawbridge) - A Confidential Computing-Aware Workload Repository.
- [enarx/steward](https://github.com/enarx/steward) - A Confidential Computing-Aware Certificate Authority.
- [confidential-containers/guest-components](https://github.com/confidential-containers/guest-components) - Confidential Containers Guest Tools and Components.
- [kinvolk/azure-cvm-tooling](https://github.com/kinvolk/azure-cvm-tooling) - Libraries and tools for Confidential Computing on Azure.
- [HyperEnclave/hyperenclave](https://github.com/HyperEnclave/hyperenclave) - An Open and Cross-platform Trusted Execution Environment.
- [mobilecoinfoundation/mobilecoin](https://github.com/mobilecoinfoundation/mobilecoin) - Private payments for mobile devices.
- [integritee-network/worker](https://github.com/integritee-network/worker) - Integritee off-chain worker and sidechain validateer.
- [capsule-corp-ternoa/ternoa-node](https://github.com/capsule-corp-ternoa/ternoa-node) - Ternoa's Node Implementation.
- [automata-network/automata](https://github.com/automata-network/automata) - Automata Network is a modular attestation layer that extends machine trust to Ethereum with TEE Coprocessors.
- [apache/incubator-teaclave](https://github.com/apache/incubator-teaclave) - Apache Teaclave (incubating) is an open source universal secure computing platform, making computation on privacy-sensitive data safe and simple.
- [scrtlabs/incubator-teaclave-sgx-sdk](https://github.com/scrtlabs/incubator-teaclave-sgx-sdk) - Rust SGX SDK provides the ability to write Intel SGX applications in Rust Programming Language. Fork of `apache/incubator-teaclave-sgx-sdk`.

### Go

- [google/go-tpm-tools](https://github.com/google/go-tpm-tools) - Go packages built on go-tpm providing a high-level API for using TPMs.
- [google/go-sev-guest](https://github.com/google/go-sev-guest) - Library to wrap the /dev/sev-guest device in Linux, as well as a library for attestation verification of fundamental components of an attestation report.
- [google/go-tdx-guest](https://github.com/google/go-tdx-guest) - Library to wrap the /dev/tdx-guest device in Linux, as well as a library for attestation verification of fundamental components of an attestation quote.
- [matter-labs/vault-auth-tee](https://github.com/matter-labs/vault-auth-tee) - Hashicorp Vault plugin for authenticating Trusted Execution Environments (TEE) like SGX enclaves.
- [usbarmory/GoTEE](https://github.com/usbarmory/GoTEE) - Go Trusted Execution Environment (TEE).
- [iotexproject/w3bstream](https://github.com/iotexproject/w3bstream) - An offchain computing layer for DePIN verifiable data computation, supporting a variety of validity proofs including Zero Knowledge (ZK), Trusted Execution Environments (TEE), and Multi-party Computation (MPC).
- [oasisprotocol/oasis-core](https://github.com/oasisprotocol/oasis-core) - Performant and Confidentiality-Preserving Smart Contracts + Blockchains.
- [hyperledger/fabric-private-chaincode](https://github.com/hyperledger/fabric-private-chaincode) - FPC enables Confidential Chaincode Execution for Hyperledger Fabric using Intel SGX.
- [Microsoft/confidential-container-demos](https://github.com/microsoft/confidential-container-demos) - Demos for running containers in confidential environments on Azure.

### CPP

- [intel/linux-sgx](https://github.com/intel/linux-sgx) - Intel SGX SDK and Platform Software (PSW) for Linux.
- [NixOS/nix](https://github.com/NixOS/nix) - Nix, the purely functional package manager.
- [microsoft/azure-tee-attestation-samples](https://github.com/microsoft/azure-tee-attestation-samples) - Trusted Execution Environment examples leveraging attestations on Azure.
- [lsds/Teechain](https://github.com/lsds/Teechain) - Teechain: A Secure Payment Network with Asynchronous Blockchain Access.
- [skalenetwork/sgxwallet](https://github.com/skalenetwork/sgxwallet) - Opensource high-performance hardware secure crypto wallet that is based on Intel SGX technology. First opensource product on Intel SGX whitelist. Scales to 100,000+ transactions per second. Currently supports ETH and SKALE, and will support BTC in the future. Sgxwallet is under heavy development and use by SKALE network.
- [hyperledger-labs/private-data-objects](https://github.com/hyperledger-labs/private-data-objects) - The Private Data Objects lab provides technology for confidentiality-preserving, off-chain smart contracts.

### C

- [openenclave/openenclave](https://github.com/openenclave/openenclave) - SDK for developing TEE applications (enclaves) across different hardware platforms (SGX, OP-TEE).
- [gramineproject/gramine](https://github.com/gramineproject/gramine) - A library OS for Linux multi-process applications, with Intel SGX support.
- [iisec-suzaki/optee-ra](https://github.com/iisec-suzaki/optee-ra) - OP-TEE Remote Attestation.
- [pietroborrello/CustomProcessingUnit](https://github.com/pietroborrello/CustomProcessingUnit) - The first analysis framework for CPU microcode.
- [deislabs/mystikos](https://github.com/deislabs/mystikos) - Tools and runtime for launching unmodified container images in Trusted Execution Environments.
- [mofanv/PPFL](https://github.com/mofanv/PPFL) - Privacy-preserving Federated Learning with Trusted Execution Environments.
- [inclavare-containers/inclavare-containers](https://github.com/inclavare-containers/inclavare-containers) - A novel container runtime, aka confidential container, for cloud-native confidential computing and enclave runtime ecosystem.

### Others

- **WASM**
  - [enarx/enarx](https://github.com/enarx/enarx) - Enarx: Confidential Computing with WebAssembly.
- **Shell**
  - [flashbots/yocto-manifests](https://github.com/flashbots/yocto-manifests) - Repo Manifests for the Yocto Project Build System for reproducible TEE builds
- **Python**
  - [ethernity-cloud/mvp-pox-node](https://github.com/ethernity-cloud/mvp-pox-node) - Ethernity Cloud Node.
- **TypeScript**
  - [tkhq/sdk](https://github.com/tkhq/sdk) - Turnkey TypeScript SDK.

## Social Media & Community

_TEEs on social media._

- **Tweet threads**
  - [@P3b7\_, Donjon Ledger analysis of Trezor Safe 3](https://x.com/P3b7_/status/1899863743036874795)
  - [@CP2426\_, focEliza Verifiable Terminal Release](https://x.com/CP2426_/status/1871929921356067282)
  - [@\_markel\_\_\_, Extraction of Intel SGX Fuse Key0](https://x.com/_markel___/status/1828112469010596347)
  - [@PratyushRT, Breakdown of the Intel SGX (TEE) breach](https://x.com/pratyushrt/status/1828183761055330373?s=46)
  - [@buchmanster, TEE, ZK, FHE and MPC](https://x.com/buchmanster/status/1816084691784720887)
  - [@buchmanster, How you win friends and TEE-fluence people - Chapter 2](https://x.com/buchmanster/status/1816443327241490662)
  - [@DistributedMarz, Flashwares Live Session](https://x.com/DistributedMarz/status/1805640541360550110)
- **Podcasts**
  - [AI Confidential](https://podcast.aiconfidential.com) - Podcast and newsletter.
- **Community**
  - [Flashbots Collective Forum](https://collective.flashbots.net/) - Discussions often touch on TEE usage for MEV mitigation and block building.
  - [Confidential Containers Community](https://github.com/confidential-containers/confidential-containers) - Open-source project enabling cloud-native confidential computing by shielding containerized workloads.
  - [Confidential Computing Consortium](https://confidentialcomputing.io/) - Linux Foundation project advancing confidential computing.
  - [Blockchains + TEEs Workshop](https://blockchainplustees.github.io/) - Academic workshop focused on the intersection of blockchains and TEEs.

## Additional Resources

- [sbellem/qtee](https://github.com/sbellem/qtee) - Exploring the physical limits of trusted hardware in the classical and quantum settings to achieve security through physics.
- [bpradipt/awesome-confidential-computing](https://github.com/bpradipt/awesome-confidential-computing) - Collection of resources on Confidential Computing.
- [erayack/awesome-sgx-blockchain](https://github.com/erayack/awesome-sgx-blockchain) - Awesome SGX and TEE on Blockchain Resources.
- [orbstack/orbstack](https://github.com/orbstack/orbstack) - Fast, light, simple Docker containers & Linux machines.
- [TEE Bible](https://www.tee3.ai/TEE-Bible-Your-First-Stop-for-TEE-in-Crypto-15eacce4724b80d1a13ae894d3927c1d) - Your First Stop for TEE in Crypto
