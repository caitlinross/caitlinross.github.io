---
title: Dissertation
layout: page
permalink: /thesis/index.html
---
<style>
img { width: 50%; margin: 0 auto; display: block; }
</style>

Thesis: Performance Analysis and Visualization of Extreme-Scale Parallel Discrete Event Simulations <br />

Discrete event simulation (DES) is one common approach to simulating computer system components, such as high performance computing networks.
Entities in the simulated system (for example, a network router) are modeled as logical processes (LPs), which communicate through the exchange of time stamped messages.
When running these simulations in parallel, we map some number of LPs to each processing element (PE) available in the simulation and use a synchronization protocol for ensuring events are processed in the correct order.
In PDES, there are two classes for synchronization protocols - conservative and optimistic.
Conservative uses some information from the model to determine when it is safe to process events.
On the other hand, optimistic allows for events to be processed speculatively and provides mechanisms to detect events processed out of order as well as to let the system recover from events processed incorrectly.

Because of the speculative processing, optimistic tends to scale better than conservative methods since optimistic methods can better take advantage of the parallelism inherent in a model.
Unfortunately, to achieve reasonable performance in optimistic mode, the simulation needs to be tuned appropriately for the model, to limit the amount of unproductive work (i.e., rolling back the system to fix events processed out of order).
Optimistic protocols work well on balanced, homogeneous models, but can suffer excessive rollbacks on complex heterogenous models that drastically degrade performance.

Optimistic PDES provides a promising approach to high-fidelity simulations of extreme-scale computing systems and there are a number of PDES simulators available, but the difficulty in performance tuning makes it difficult for it to be used by anyone not already working in PDES.
In my thesis, I am working on developing tools that will help PDES users understand performance issues in their simulation, as well as debug certain aspects of their simulations.
Ideally this work will also allow us to develop dynamic tuning capabilities available at runtime for our simulator, which will make PDES further accessible.

I specifically work with [Rensselaer's Optimistic Simulation System](https://carothersc.github.io/ROSS) (ROSS, no relation to my name).
ROSS can run simulations in both conservative and optimistic modes, though I focus on optimistic execution.
I have developed a dynamic instrumentation layer for ROSS that can collect detailed data about the simulation engine and the model being simulated.
We can use this data to create visualizations that help us better understand the behavior of the simulations and find performance bottlenecks.
Early work in this area has been published in [PMBS '16](http://www.dcs.warwick.ac.uk/pmbs/pmbs/PMBS/Welcome.html).

Paper: [Visual Data-Analytics of Large-Scale Parallel Discrete-Event Simulations](../papers/ross-pmbs16.pdf)

The instrumentation has the potential to generate a lot of data, so currently I am working on an in situ analysis system for ROSS.
This system will stream data to visualization tools built by our collaborators at UC Davis, and it will also need to perform some data reduction so all data is not transferred over the network.
This component will need to intelligently decide which performance data should be streamed in high resolution, and which data is okay to be streamed as global aggregates.
As this component is further developed, I will update this section.
