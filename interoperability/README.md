# Interoperability / Onchain SLD

## Objective

The Handshake blockchain only deals with the root zone i.e. Top Level Domains (TLDs). As the root is referral only, all domains and subdomains along with their records must be stored and served off-chain, like regular DNS.

This task is to explore different ways and implement a solution to also store Second Level Domains (SLDs) on chain.

This project has a bounty for $250 USD

## Requirements

1. SLD registrations and ownership should be on the Handshake chain
2. Owners should be able to set DNS records
3. hsd resolver should be able to resolve these records

## Deliverables

1. Either a working/resolving SLD on a test network, or a test script covering all requirements above
2. A write-up of the solution and how it works



Useful docs

- [HIP05](https://github.com/handshake-org/HIPs/blob/master/HIP-0005.md) - Handshake Improvement Proposal (HIP) 05 - Name data standard for alternative namespace resolution
- [HIP06](https://github.com/handshake-org/HIPs/blob/master/HIP-0016.md) - Handshake Improvement Proposal (HIP) 16 - Escher Update Chains for decentralized subdomains
- [HNS.ID Contracts](https://docs.hns.id/contracts) - HNS.ID contracts for their decentralized subdomains using Optimism L2