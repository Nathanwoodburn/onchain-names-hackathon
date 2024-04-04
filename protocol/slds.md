# SLDs on Handshake

## Objective

The Handshake blockchain only deals with the root zone i.e. Top Level Domains (TLDs). As the root is referral only, all domains and subdomains along with their records must currently be stored and served off-chain, like regular DNS.

With only DNS, all subdomains are still owned by the parent zone (TLD in case of Handshake). Traditional registry setups are centralized and the Second Level Domains (SLDs) issued are not provably transferred to the owners on chain, they only get access to update records.

This task is to explore different ways and build a proof of concept of trustless SLD ownership on Handshake, without reliance on centralized registries and DNS hosts.

This project has a bounty for $1000 USD

Prior work:

- HIPR Aliasing https://github.com/lukeburns/hipr-aliasing
- Escher https://hsd-dev.org/HIPs/proposals/0016/

## Requirements

1. SLD registrations and ownership should be on the Handshake chain
2. Owners should be able to set DNS records and use their SLDs for websites, etc. just like TLDs
3. A resolver (like hsd or hnsd) should be able to resolve these records

## Deliverables

1. Either a working/resolving SLD on a test network, or:
test scripts covering all requirements above
2. Documentation on how the protocol works, how to set up TLDs with this protocol, how to register and use SLDs

## Evaluation Criteria

1. Adherence to task requirements and specifications
2. Security and robustness of the implemented solution
3. Overall creativity and innovation