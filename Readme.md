# KOB PIU

## Abstract

KochiOrgBook public identity utility, an identity network for the city of Kochi. All the DIDs will be hosted upon the identity network. This network which is going to be the 1st layer of ToIP tecnology stack. The first layer is mainly for blockchains and distributed ledgers. The identity utility network is similar to that of Sovrin network.

## Dependent Projects
TBD
## Motivation

As Individuals and Organizations use variety of credentials and documents for different purpose and we share those documents in internet. These credentials and documents serve as a unique identifiers which gives our communication addresses, ID Numbers and other personal informations. Sharing these personalized information in the Internet is not safe, attackers can get the information and can use them.  So we are using a new type of gloablly unique identifiers called DIDs which helps individuals and organizations to generate our own identifiers using systems we trust, and to prove control of those identifiers (authenticate) using cryptographic proofs (for example, digital signatures).
And at the same time the users have independent existence. If we are using the identities digitally it must be long lived and it is very easy for transportation. The user's rights are protected while using DIDs. 
## Status of the project

Incubation state.

## Solution

Decentralized Identifiers (DIDs) are a new type of identifier that enables verifiable, decentralized digital identity. DID is the idea that you control your own data, you control when and how it is provided to others and when it is shared, It is done so in a trusted way. In contrast to typical, identifiers, DIDs have been designed so that they may be independent of centralized registries, identity providers, and certificate authorities. Individuals or Organizations can prove control over it without requiring permission from any other party.DIDs provide URIs that makes the interaction with specific documents.Each DID document can express cryptographic material, verification methods, or services, which provide a set of mechanisms enabling a DID Controllers to prove control of the DID. Services enable trusted interactions associated with the DID subject. A DID might provide the means to return the DID subject itself, if the subject is an information resource such as a data model. The  participants of Identifiers are Issuer, Holder and the Verifier. The Issuer can issue the documents and Prover can prove their identity to the verifier without interacting with the issuer. 

The Holder can pass the valid DID to a piece of software called a DID resolver, It works like a browser given a URL, resolving the DID and return DID subject. It contains public keys whose private keys are held by the entity that controls the DID and service endpoints that enable communication with that entity.

If a central authority controls your identifiers they can remove or delete those identifiers, but if you are the controlling there will not be such issue. A DID can never be removed, so deleting a DID means no longer responding to requests for proof of control of the DID.

## Contributors
[Anjana M P](https://github.com/Anjana-mp/KOBPIU/blob/master/Readme.md)

## Testing the project

TBD

## Refernces
*    https://www.edx.org/professional-certificate/linuxfoundationx-developing-blockchain-based-identity-applications
* www.w3.org/TR/did-core
