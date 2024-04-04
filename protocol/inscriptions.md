# Inscriptions on Handshake

## Objective

While Handshake’s current Resource data is meant to store DNS records, each name can actually store upto 512 bytes of arbitrary data. The task here is to make use this space to store other types of data (text, pictures, links, etc.)

Inpsiration can be found from Bitcoin’s Ordinals (https://docs.ordinals.com/inscriptions.html) like they way they store mime-type and content. (but since Handshake doesn’t support Taproot, directly porting Ordinals will not be possible.)

This project has a bounty for $1000 USD

## Requirements

- Should be able to select and inscribe content with an owned name
- Should be able to view all inscriptions on chain

## Deliverables

- A way to easily inscribe content on a name
- An indexer for the chain that reads all inscriptions
- A website to view all inscriptions from the indexer
- Technical documentation on how data is stored on chain

## Evaluation Criteria

1. Adherence to task requirements and specifications
2. Planning for future extensions
3. Overall creativity and innovation