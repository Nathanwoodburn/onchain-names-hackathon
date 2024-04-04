# Interoperability / Onchain SLD

## Objective

The Handshake blockchain only deals with the root zone i.e. Top Level Domains (TLDs). As the root is referral only, all domains and subdomains along with their records must be stored and served off-chain, like regular DNS.

This task is to explore different ways and implement a solution to also store Second Level Domains (SLDs) on chain.

## Requirements

1. SLD registrations and ownership should be on the Handshake chain
2. Owners should be able to set DNS records
3. hsd resolver should be able to resolve these records

## Deliverables

1. Either a working/resolving SLD on a test network, or a test script covering all requirements above

## Evaluation Criteria (TODO: should this be public?)

1. Adherence to task requirements and specifications
2. Security and robustness of the implemented solution
3. Balance of decentralization and practicality [TODO: reframe]
4. Overall creativity and innovation



Useful docs

- [HIP05](https://github.com/handshake-org/HIPs/blob/master/HIP-0005.md) - Handshake Improvement Proposal (HIP) 05 - Name data standard for alternative namespace resolution
- [HIP06](https://github.com/handshake-org/HIPs/blob/master/HIP-0016.md) - Handshake Improvement Proposal (HIP) 16 - Escher Update Chains for decentralized subdomains