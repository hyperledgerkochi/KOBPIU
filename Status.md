# Topics Covered KOB PIU
## KOB PIU
KochiOrgBook public identity utility, an identity network for the city of Kochi. All the DIDs will be hosted upon the identity network. This network which is going to be the 1st layer of ToIp tecnology stack.
## ToIp Stack
### _Layer 1_
This layer is mainly for blockchains and distributed ledgers. It is a layer of public utilities for decentralized identifiers (DIDs).
### _Layer 2_
This layer is for peer DID and DID to DID connections and communications.
### _Layer 3_
The purpose of third and fourth layer is to establish human trust between peers, trust between individuals and organizations and the thing with which they interact.
### _Layer 4_
Layer Four is the layer where humans interact with applications in order to engage in trusted interactions that serve a specific business, legal, or social purpose. 
## Verifiable Credentials
Verifiable credentials are cryptographically constructed so that a presentation proves the 4 key attributes of all credentials. The 4 key attributes are:
* Who issued the credential
* The credential was issued to the entity presenting it
* The claims were not tampered
* The credential has not been revoked
When a reciever recieves a presentation from a holder they use the information from a blockchain to perform the cyptographic calculations necessary to prove the 4 attributes.
## SSI (Self Soverign Identifiers)
* The idea that you control your own data.
* No central authority
## Decentralized Identifiers (Layer 1)
Special kind of identifiers that are created by their owner, independent of any central authority. Adapting the decentralized systems to be the base layer of the ToIP stack required a new type of globally unique identifier called a Decentralized Identifier (DID).
DIDs are defined by an RFC 3986-compliant URI scheme designed to provide four core properties:
1. Permanence. A DID effectively functions as a Uniform Resource Name (URN), i.e., once assigned to an entity (called the DID subject), a DID is a persistent identifier for that entity that should never be reassigned to another entity.
2. Resolvability. A DID resolves to a DID document—a data structure (encoded in JSON or other syntaxes) describing the public key(s) and service endpoint(s) necessary to engage in trusted interactions with the DID subject.
3. Cryptographic verifiability. The cryptographic material in a DID document that enables a DID subject to prove cryptographic control of a DID.
4. Decentralization. Because a DID is cryptographically generated and verified, it does not require a centralized registration authority such as those needed for phone numbers, IP addresses, or domain names today.
### **DID Methods**

Like the URN specification, the DID specification also defines a generic URI scheme which is in turn used for defining other specific URI schemes. With DIDs, these are called DID methods. Each DID method is defined by its own DID method specification that must include:

* The target system (technically called a verifiable data registry) against which the DID method operates. In the ToIP stack this is called a utility. Note that a utility is not required to be implemented as a blockchain or distributed ledger. DID methods can be designed to work with any type of distributed database, file system, or other system that can anchor a cryptographic root of trust.
* The DID method name.
* The syntax of the DID method-specific string.
* The CRUD (Create, Read, Update, Delete) operations for DIDs and DID documents that conform to the specification.

Here we are using permissioned ledger which is a DID Method Registry similiar to sovrin. There are different types of method registerys like Permissionless Blockchain, Distributed file systems, Ledgerless P2P networks.
### **Utility Governance Frameworks**
All ToIP architecture requires is that the governance model conform to the requirements of the ToIP Governance Stack to support both interoperability and transitive trust. This includes transparent identification of the governance authority, the governance framework, and participant nodes or operators; transparent discovery of nodes and/or service endpoints; and transparent security, privacy, data protection, and other operational policies.

Utility governance frameworks that conform to the ToIP Governance Stack model will support standard roles for all types of utility governance authorities. For example, the role currently supported by public-permissioned utilities such as those based on Hyperledger Indy include:

* Transaction Authors: initiate transactions
* Transaction Endorsers: permission transactions for Transaction Authors
* Stewards: operate a node of the ledger
## ZKP (Zero Knowledge protocol)
Proving attributes about an entity without exposing all other details about that entity.
## Selective Disclosure
Proving pieces of info without presenting the underlying data.
## Agents and Wallets
Software that you use to process verifiable credentials and DIDs. 
Software that interacts with other entities.
## Hyperledger Indy
Hyperledger Indy is the implementation of distributed ledger. Indy is mainly for storing blockchain elements and provides verifiable credentials. Blockchain is a decentralized source of trust for publicaly available information.

What is on Blockchain?

* Public DIDs
* Issuer's Public key
* Credential Schema

What is not on Blockchain?

* Pairwise DIDs
* Credentials
* Prover
* Private keys