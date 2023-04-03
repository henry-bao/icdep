# What needs fixing in the Index Card Data Exchange Protocol?

This repo answers the following questions:

- [Anti-Duplication](anti-dupe.md): How can we ensure that each card is received once and only once?

- [Extension](extension.md): How can we add additional features to the protocol without breaking previous functionality?

    Consider:
  - Send to any individual on the whole UW campus
  - Specify whether contents are ASCII text, Unicode text, or binary values
  - Keep a record of what nodes the card has passed through.

- [Administration](admin.md): How can we send commands ("SLEEP", "RESTART", "ARE-YOU-THERE", etc) to individual nodes in the network, rather than treat them as pass-through intermediaries?
