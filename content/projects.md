---
title: "Projects"
date: 2019-12-22T11:49:22+01:00
draft: true
---

## R2P2
Our work on ZygOS revealed the mismatch between TCP's streaming semantics and RPCs' message-oriented semantics. R2P2 (Request Response Pair Protocol) is a transport protocol specifically designed for datacenter RPCs. It exposes a request and response abstraction, as opposed to streams or messages, and allows for in-network policy enforcement based on software and hardware middleboxes. We explored several RPC policies on top of R2P2 such as fault-tolerance in [HovercRaft](/pubs/hovercraft.pdf) and SLO-aware admission control in [SVEN](/pubs/sven.pdf).

<i class="fab fa-github"></i> [Source Code](https://github.com/epfl-dcsl/r2p2)

## Lancet
Doing research in the μs-scale requires tools with the equivalent accuracy. Lancet is a self-correcting tool designed to measure the open-loop tail latency of μs-scale datacenter applications with high fan-in connection patterns. It leverages NIC-based timestamping to improve measurement accuracy and it implements a robust experiment methodology based on online statistical testing to drive the experiment.

<i class="fab fa-github"></i> [Source Code](https://github.com/epfl-dcsl/lancet-tool)

## ZygOS
ZygOS is a datacenter operating system that specializes in serving μs-scale RPCs with strict tail-latency SLOs on top of TCP. It implements a work-conserving scheduler that depends on work-stealing and imitates the behavior of a single queue system.

<i class="fab fa-github"></i> [Source Code](https://github.com/ix-project/zygos)
