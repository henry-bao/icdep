# Extension

To add more features without breaking existing functionality, we can implement a system of request headers for each index card. Request headers provide metadata about the card, such as intended features or specific data formats. This approach allows nodes to understand and process the content accordingly without affecting the core protocol. Nodes that don't recognize a specific header will ignore it and maintain compatibility with existing protocol features so that new features can be added seamlessly without disruption to current functionality.

Example use cases:

- Send to any individual on the whole UW campus: Introduce a "GeoLocation" header that contains location information for routing purposes. Nodes with updated functionality can use this header to route the card effectively.
- Specify whether contents are ASCII text, Unicode text, or binary values: Introduce a "ContentType" header that indicates the content format. This allows nodes with updated functionality to parse and understand the content properly.
- Keep a record of what nodes the card has passed through: Introduce a "NodeTrace" header that logs each node the card travels through. Nodes capable of handling this header can contribute to the log and use it for tracking purposes.
