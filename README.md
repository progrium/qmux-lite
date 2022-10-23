# qmux-lite
simpler wire protocol for multiplexing connections or streams into a single connection, based on a subset of [qmux](https://github.com/progrium/qmux).

qmux-lite is the qmux protocol without the window flow-control mechanism. This makes it much easier to implement while still working in situations where flow-control is less necessary (local IPC, in-memory). A qmux-lite implementation can easily be upgraded to qmux by adding the removed window related messages and flow-control mechanism. 

# [Specification](https://github.com/progrium/qmux-lite/blob/main/SPEC.md)