# Anti-Duplication

To prevent duplicate cards from being received in the Index Card Data Exchange Protocol, we can assign each card with UUID for each card created. Before a node accepts a new card, it should check its internal card registry to see if the UUID already exists. If the UUID is found in the registry, the card is considered a duplicate and can be safely discarded. If the UUID is new, the node can process the card and store the identifier in the registry for future reference.
