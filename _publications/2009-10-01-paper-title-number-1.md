---
title: "IIBLAST: Speeding Up Commercial FPGA Routing by Decoupling and Mitigating the Intra-CLB Bottleneck"
authors: "Shashwat Shrivastava, Stefan Nikolić, Chirag Ravishankar, Dinesh Gaitonde, Mirjana Stojilović"
collection: publications
permalink: /publication/iccad23
excerpt: 'This paper proposes a new routing algorithm for AMD FPGAs, which turns one of their architectural features---an extremely sparse logic block input interconnect structure---from a major source of routing runtime expenditure into an advantage that allows straightforward parallelization. However, the main advantage is brought by the overal reduction in the amount of work that the router has to do. This reduction is further increased by a simple architectural modification inspired by the new algorithm. The paper was a result of a collaboration with Chirag Ravishankar and Dinesh Gaitonde, which also allowed the experiments to be conducted in a very realistic setting.'

date: 2023-11-02
venue: "ICCAD'23"
doi: "10.1109/ICCAD57390.2023.10323897"
abstract: "We identified that in modern commercial FPGAs, routing
signals from the general interconnect to the configurable logic blocks
(CLBs) through a very sparse input interconnect block (IIB) represents
a significant runtime bottleneck. This is despite academic research usually
altogether neglecting the runtime of last-mile routing through the IIB.
To alleviate this bottleneck, we combine computer-aided design (CAD)
and FPGA architecture enhancements. We propose a multi-stage FPGA
routing approach, based on the premise that once the signals are legally
routed in general interconnect—only reaching the inputs of the IIB, but
not the final targets—the remaining last-mile routing through the IIB
can be completed efficiently and independently for each FPGA tile. Then,
the final routing solution can simply be built by joining the previously
obtained partial solutions. However, we observe that some properties of
modern IIB architectures limit the success rate of the intra-CLB routing,
creating the need for revisiting the routing in the general interconnect
and inevitably impairing the multi-stage routing runtime gains. We show
that an enhanced IIB architecture mitigates the issue at a minimal cost.
With ISPD16 benchmarks and an FPGA architecture model closely
resembling AMD UltraScale FPGAs, we demonstrate the dominant
contribution of last-mile routing to the router’s runtime. After applying
our multi-stage routing approach and the proposed enhancements, we
show that the observed bottleneck can be mitigated, resulting in 4.94×
faster routing on average.
Index Terms—CLB, congestion, FPGA, IIB, routing"
---

[Author's local PDF copy of paper](http://stefannikolicns.github.io/files/Shrivastava_et_al___IIBLAST_Speeding_Up_Commercial_FPGA_Routing_by_Decoupling_and_Mitigating_the_Intra_CLB_Bottleneck___2023.pdf)
