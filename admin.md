# Administration

For sending commands to individual nodes, we can introduce a "command" message type that only targets specific nodes. These command messages would be different from regular messages passed through intermediaries. Nodes should be programmed to recognize command messages and execute the accompanying instructions like "SLEEP," "RESTART," or "ARE-YOU-THERE". When a node receives a card containing this type of command, it checks if the target UID matches its own. If it does, the node executes the command. Otherwise, the card is passed to the next node, as usual.
