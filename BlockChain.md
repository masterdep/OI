# Criptomoedas & BlockChain

## Applications
Cryptography and blockchain technology offer unique advantages that make them valuable in various projects, particularly in those requiring trust, security, and decentralized record-keeping. Here's why they are used and where they shine:

### Cryptography:

Data Security: Cryptography ensures the confidentiality, integrity, and authenticity of data. It encrypts sensitive information, making it unreadable to unauthorized users.
Secure Communication: It enables secure communication channels, ensuring that only intended recipients can access and understand messages.
Authentication and Verification: Cryptography provides mechanisms to verify the authenticity of data sources and ensure data hasn't been tampered with.
Blockchain:

### Decentralization: 

Blockchain's distributed and decentralized nature eliminates the need for a central authority. It enables trust in a network of untrusted participants by consensus mechanisms.
Immutable Record Keeping: Once data is recorded on a blockchain, it's extremely challenging to alter or delete, ensuring a tamper-proof ledger.
Transparency and Traceability: The transparent nature of blockchains allows for traceability and audit trails, fostering trust in transactions and data.

Use Cases:
- Finance and Banking: Blockchain's transparent and secure ledger system is beneficial for financial transactions, ensuring secure and traceable transactions without the need for intermediaries.
- Supply Chain Management: It's used to track and authenticate the journey of goods from their origin to consumers, ensuring transparency and preventing counterfeiting.
- Healthcare: Blockchain ensures the secure sharing of patient data among different healthcare providers while maintaining patient privacy.
- Voting Systems: Provides secure and transparent voting systems by ensuring integrity, authenticity, and tamper-proof records.
- Smart Contracts: Blockchain facilitates self-executing contracts, automating and enforcing contract terms without intermediaries.

Projects requiring transparency, security, and decentralized trust mechanisms often find significant value in using blockchain technology coupled with cryptography. Industries where trust is a critical factor, and where traditional centralized systems may lack transparency or security, are prime candidates for blockchain integration

## Cryptocurrencies Concepts

### Hashes
- Mapping function
- Collision Resistant
  - X and Y different means H(X) different than H(Y)
- Random Distribution
  - You don't know where the function will map on the Image
- Non invertible
  - Have only H(Y) you can't recover Y

Hashes are functions, i.e. maps a domain to an image. In the case of cryptocurrencies, the domain is the set of all possible transactions and the image is the set of all possible hashes. The hash function is a one-way function, i.e. it is easy to compute the hash of a transaction, but it is very difficult to find a transaction that has a given hash. The hash function is also collision-free, i.e. it is very difficult to find two transactions that have the same hash.

The domain is larger than image. This means that there are more possible transactions than possible hashes. This means that there are many transactions that have the same hash. This is called a hash collision. The hash function is **collision resistant**, i.e. it is very difficult to find two transactions that have the same hash, it is very difficult to find two transactions that have the same hash. 

#### How are hashes used in cryptocurrencies?
- Commitments
- Information hiding
- Puzzles




1. Cryptocurrencies and Blockchain Technology:
Cryptocurrencies are digital or virtual currencies that use cryptographic techniques to secure financial transactions and control the creation of new units. They rely on blockchain technology, a decentralized ledger system that records all transactions across a network of computers. Blockchain ensures transparency, security, and immutability of transaction records.

2. Consensus Mechanisms:
Consensus is critical in the world of cryptocurrencies. It involves agreements on:

Rules: Determining what is considered valid (e.g., transaction rules).
History: Agreements on the blockchain’s transaction history, coin ownership, and immutability.
Value: Deciding the value of a cryptocurrency, often influenced by market forces and game theory.
3. Interactions of Consensus:
These three consensuses—rules, history, and value—interact:

They influence each other and drive behaviors within the cryptocurrency ecosystem.
Any compromise in one consensus can destabilize the entire system.
4. Rule Adherence and Evolution:

Cryptocurrencies operate on open-source software governed by foundations.
The rules are written in algorithms for precise functionality and transparency, leading to better rules.
Rule evolution occurs through proposals (such as Bitcoin Improvement Proposals - BIPs) that undergo community consensus.
5. Forks and Disagreements:

Disagreements within cryptocurrency communities can lead to forks, splitting the blockchain into different versions.
Forks can be hard (contentious) or soft (non-contentious), affecting the community differently and sometimes leading to the creation of new coins.
6. Government Regulation and Motivation:
Governments are motivated to regulate cryptocurrencies due to concerns such as:

Tax avoidance and evasion of capital controls facilitated by cryptocurrencies.
The use of cryptocurrencies in illegal activities like kidnapping, exchanges of illegal items, and corruption.
Privacy concerns arising from the immutable nature of blockchain, which can permanently record sensitive information.
7. Specific Regulations - Bitlicense and Brazil's Case:

The Bitlicense, introduced in New York in 2014, regulates various cryptocurrency activities and requires licenses, cybersecurity measures, and compliance.
Brazil has been discussing similar regulations, aiming to address their specific context, but the process has faced interruptions due to legislative cycles.
These regulations aim to strike a balance between fostering innovation in the cryptocurrency space while ensuring consumer protection, market integrity, and regulatory compliance. They continue to evolve to adapt to the changing landscape of cryptocurrencies and their implications on financial systems and society.

## Primitives

Integrity:
This refers to the assurance that data hasn't been altered or tampered with. Cryptographically, integrity can be verified by using hash functions to generate a fixed-size "fingerprint" or hash of the original data. Any change in the data, even a tiny alteration, will result in a vastly different hash.

Authenticity:
Authenticity ensures that the origin of data can be verified. It's about confirming that data comes from a genuine or trusted source. However, ensuring authenticity in historical contexts can be challenging, as demonstrated by cases like Denis Vrain-Lucas forging historical letters purportedly from famous figures.
Temporality (or Temporality Verification):

This aspect is concerned with verifying when certain data was created or existed. For example, in the context of option-backdating scandals, it's about identifying when certain financial data or events occurred.
Interactions Between Integrity, Authenticity, and Temporality:

These cryptographic objectives interact to provide comprehensive data assurance. Ensuring integrity through hashing techniques aids in verifying the authenticity of data sources. Temporality verification can be linked to authenticity, confirming when data was created or when specific events occurred, bolstering the authenticity claim.
Cryptography Basic Principles:

Hard Math Problems: Cryptography relies on complex mathematical problems that are computationally infeasible to solve without specific information or keys.
Security Tool, Not Panacea: Cryptography is a security tool, not a solution to all security challenges. Its effectiveness depends on its proper implementation and usage within an overall security framework.
Verifying Integrity with Hash Functions:

Issues: Storing originals for comparison, especially with large data like a 4K movie, is impractical.
Solution - Hash Functions: Hash functions create fixed-size "fingerprints" (hashes) of data. Even a small change in the original data results in a significantly different hash value. This provides an efficient way to verify integrity without storing the original data.
Hash Functions Properties:

Preimage Resistance: It's hard to find the original input data from its hash.
Second Preimage Resistance: Given input data and its hash, it's hard to find different input data with the same hash.
Collision Resistance: It's difficult to find two different inputs that produce the same hash.
Avalanche Effect: Minor changes in input result in drastically different hash values, ensuring unpredictability.
Hash functions serve as essential tools in ensuring data integrity and are the backbone of many cryptographic protocols due to their properties like collision resistance and preimage resistance. They provide a reliable means to verify data integrity without needing to store the original data for comparison.

## Anonimity

Anonymity Basics: Cryptocurrencies like Bitcoin are often considered anonymous because they don’t use names; instead, they use complex cryptographic keys. However, they're better described as pseudonymous - transactions aren't tied to real identities but are visible on a public ledger.

### Pseudo-anonymity vs. True Anonymity:

Pseudo-anonymity involves using random addresses, but repeated use can be traced back to you through various means.
Achieving true anonymity would mean using a different address every time you transact, which is quite challenging.
Unlinkability: Making it tough to connect different transactions or addresses to the same person. Factors like KYC standards at exchanges and other off-chain information make this difficult.

### Why Anonymity Matters:

Public transactions on blockchains compromise privacy.
While anonymity is essential for lawful purposes, it can be misused for illegal activities like money laundering.

### Best Practices for Anonymity in Bitcoin:

Using fresh addresses for receiving.
Being mindful of address management and disposal.

### Deanonymization Techniques:

Clustering addresses, mapping change addresses, and using off-chain information like IP addresses for identification.

### Enhancing Anonymity:

Mix Nets: Used to anonymize transactions by mixing them together. TOR, known for anonymity in browsing, is an example.
Mixers in Cryptocurrencies: Systems like Zcash and Monero aim to enhance privacy by obfuscating transaction details.

### Conclusions:

Achieving true anonymity is tough due to various factors like regulations, data leaks, and the public nature of blockchains.
Cryptocurrencies with enhanced privacy features, like Zcash and Monero, aim to solve these issues.
So, while cryptocurrencies provide a degree of anonymity, achieving complete anonymity is challenging due to various factors. However, technologies like Mix Nets and privacy-centric cryptocurrencies continue to evolve to address these concerns.

## Altcoins
#### Namecoin:

Introduction: Created in 2011, it was the first altcoin and aimed to replace the traditional DNS system.
Domain System: Allows the creation of decentralized domains ending in ".bit", providing a censorship-resistant domain registration system.
Features: Offers low-cost domain registration, transfer using coins, and no renewal fees. However, domains must be updated every 6 months to stay active.
Merge-Mining: Introduced the concept of merge-mining, allowing miners to mine both Bitcoin and Namecoin simultaneously.

#### Litecoin (LTC):

Launch: Developed in 2011, referred to as the "silver" to Bitcoin's "gold."
GPU Resistance: Initially aimed to be GPU-resistant to prevent mining centralization but later faced GPU mining dominance.
Technical Aspects: Uses the Scrypt hashing algorithm, which aimed to be more memory-intensive, and has a faster block generation rate of 2.5 minutes.

#### Peercoin (PPC):

Innovation: Introduced in 2012 as the first cryptocurrency with a Proof-of-Stake (PoS) mechanism alongside Proof-of-Work (PoW).
Hybrid Consensus: Mixes PoW for minting new coins with PoS for network security. PoW blocks aren't included in the longest chain calculation.
Centralization Concerns: Had a feature where administrators signed checkpoints, compromising decentralization.

#### Dogecoin (DOGE):

Humorous Origin: Born in 2013 as a playful cryptocurrency based on a popular internet meme.
Marketing Initiatives: Conducted successful marketing campaigns, sponsoring events like NASCAR and supporting the Jamaican Bobsled team.
Early Issues: Initially faced challenges due to random block rewards, causing fluctuations in mining profitability and impacting inflation.

#### Ethereum (ETH):

Smart Contracts: Emerged in 2013, Ethereum introduced smart contracts, enabling developers to create decentralized applications (dApps) using a Turing-complete programming language.
Ether (ETH): The native cryptocurrency used for executing smart contracts and transactions on the Ethereum network.
Applications: Smart contracts allow for a wide range of applications, from decentralized finance (DeFi) and token creation to decentralized governance and more.

#### Monero (XMR):

Privacy Focus: Established in 2014, Monero prioritizes privacy and anonymity.
Privacy Features: Implements ring signatures, stealth addresses, and obfuscated distributed ledger technology to ensure untraceable transactions.
Ransomware Association: Due to its privacy features, it has been utilized in ransomware attacks, as transactions cannot be easily traced.

#### Cardano (ADA):

Secure Proof-of-Stake: Launched in 2015, Cardano emphasizes a provably secure PoS algorithm called Ouroboros, validated using formal verification methods.
Layered Structure: Features a multi-layered architecture with the settlement layer for transactions and the control layer for smart contracts and regulatory features.
Focus on Scalability: Aims to address scalability, interoperability, and sustainability issues prevalent in existing blockchain networks.

## Regulation and Resilience
### Consensus in Cryptocurrencies:
- Consensus about Rules: This refers to the agreement among nodes (computers) in a cryptocurrency network regarding what constitutes a valid block. This consensus involves reaching an agreement on the transactions within a block and how nodes behave, particularly in solving cryptographic puzzles to validate transactions.

- Consensus about History: This consensus involves agreeing on the blockchain's history, including which transactions are recorded, the creation of new coins (minting), and who owns these coins. Immutability is a crucial aspect; once transactions are added to the blockchain, they cannot be altered.

- Consensus about Value: Determining the value of a cryptocurrency is a market-driven consensus. The value is influenced by factors like demand, supply, market sentiment, utility, and adoption.

### Interactions Among Consensuses:
These interactions are influenced by game theory principles:

- Rules determining History: The agreed-upon rules dictate the transactions and events that are recorded on the blockchain.
- History determining Value: The recorded history of transactions influences the perceived value of a cryptocurrency. Investors often base their decisions on historical performance.
- Value driving Incentives: The perceived value drives incentives for miners to validate transactions and maintain the network.

### Evolution of Rules and Disagreements:
Rules in cryptocurrencies evolve through proposals like Bitcoin Improvement Proposals (BIPs). These proposals outline changes, rationale, and specifications, requiring consensus among the community for implementation.
Disagreements among the community can lead to forks, where the blockchain splits into two separate chains, often due to conflicting visions or proposed changes.

### Government Regulation:
Governments regulate cryptocurrencies due to various concerns:

- Avoiding Tax Evasion and Capital Control: Cryptocurrencies can enable individuals to move funds across borders and avoid taxes, leading to concerns about capital control evasion.
- Criminal Activities: There are concerns about cryptocurrencies being used for illegal activities like kidnapping, drug trafficking, bribery, and corruption.
- Privacy Concerns: Some laws require keeping certain information private, but once published on the blockchain, it's immutable.

### Real-World Regulation and Anti-Money Laundering:
Regulations aim to prevent large-scale financial crime by targeting money laundering, underground economies, and organized crime.

Strategies like "Follow the Money" and KYC (Know Your Customer) are used to track and prevent illicit financial activities.

Regulation Rationale and Examples:

Regulations aim to address past failures and protect against risks associated with cryptocurrencies.

Examples like New York's Bitlicense and ongoing discussions in Brazil demonstrate efforts by governments to regulate cryptocurrency activities, ensuring transparency, security, and compliance within their specific contexts.

Brazil's ongoing discussions, including those in the lower chamber and bi-chamber, highlight the country's efforts to draft specific regulations that suit their unique context, similar to New York's Bitlicense. These regulations seek to balance the potentials of cryptocurrencies while addressing potential risks and illegal activities associated with them.


## Hyperledger

### Hyperledger Fabric Characteristics:
- Open Source Distributed Ledger Platform: Initiated by Linux Foundation involving 35 organizations and over 200 developers.
- Modular and Configurable Architecture: Supports consensus protocols, cryptographic libraries, identity and key management, smart contracts, and databases.
- Private and Permissioned: Launched in 2015, Fabric allows Membership Service Providers (MSPs) using PKI with X.509 certificates for identification.
- Pseudo-Anonymity (IDEMix): Fabric provides a level of anonymity for users.

### Network Elements in Hyperledger Fabric:
- Components: Including chain codes, network configuration files, channels, ledgers, organizations, orderers, peers, certification authorities, and consortiums.
- Network Configuration (NC): The configuration block that sets up network elements and information.
- Organization (R): Represents entities defined in the network configuration, grouping participants with similar permissions.
- Orderer (O): Manages transaction consensus, allowing new participants and setting configurations.
- Consortium (X): Formed by multiple network organizations to transact data.
- Channel (C): Ensures data isolation and confidentiality, communicating with network components independently of network changes.
- Peer (P): Holds a copy of the ledger and executes/supervises smart contracts.
Chaincode (S): Installed on a peer before invoking by client applications, defining access to the ledger.
- Ledger (L): Physically hosted on peers, storing transaction states of chain codes.
- Certificate Authority (CA): Issues certificates for authentication and access permissions.
- Client Application (A): Uses certificates for authenticating transaction proposals and constructing transactions.

### Transaction Flow in Hyperledger Fabric:
- Transaction Request: Initiated by a client application and verified by its identity and application permissions.
- Verification and Execution: Checks permissions for reading or modifying ledger data.
- Simulation and Validation: Simulates the transaction execution to ensure validity and checks the current state of the blockchain.
- Ordering and Block Creation: Orders transactions and creates blocks, updating peers' ledgers.
- Blockchain Update: Incorporates the new block into the blockchain structure.
