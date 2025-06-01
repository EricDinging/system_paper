# RECCL: optimizing collective algorithms for reconfigurable optical networks

## Summary

- Propose collective sketch and reconfigurable network model.
- Minimize communication overhead by reconfiguring communication relationships through communicator and buffer reordering.
- Reconfigure the communication pattern of collective algorithm to dynamically changing network topologies

## Pros
- Fast rank-reordering search

## Cons
- Link speed is slow
- Assume traffic agnostic network reconfiguration
- Assumes every server is connected to all OCSes. And no details about intra-server topology and NIC.
- Only operate on static network.
- OCS bandwidth is shared across multiple applications


## Future work
- Codesign collective algorithms with the schedule of OCSes
- Reduce collective reconfiguration latency by knowing the possible network topology beforehand.

