---
title: Research 
layout: page
permalink: /research/index.html
---
<style>
img { width: 50%; margin: 0 auto; display: block; }
</style>


### Research Experience, Internships, and Projects

#### Graduate Research Assistant, RPI, Troy, NY

##### August 2014 - Present

Advisor: [Chris Carothers](http://www.cs.rpi.edu/~chrisc/) <br/>
Thesis: Performance Analysis and Visualization of Extreme-Scale Parallel Discrete Event Simulations <br />

My dissertation is largely focused on developing an in situ analysis system that can be used for parallel discrete event simulations (PDES) to assist in understanding performance phenomena that occur in these simulations.
With the help of this analysis system, I will be analyzing the simulation performance of several HPC network topology models that are provided by the [CODES](http://www.mcs.anl.gov/research/projects/codes/) framework built on top of the [ROSS PDES framework](https://carothersc.github.io/ROSS).

My preliminary work in this area resulted in a paper published in [PMBS '16](http://www.dcs.warwick.ac.uk/pmbs/pmbs/PMBS/Welcome.html).
This work involved the development of an instrumentation layer for ROSS.
The performance data collected from this instrumentation was then used in a visualization tool developed by collaborators at UC Davis to gain insight in to performance behaviors related to the rollback mechanism found in optimistic PDES.

Paper: [Visual Data-Analytics of Large-Scale Parallel Discrete-Event Simulations](../papers/ross-pmbs16.pdf)

In the past, I've worked on a model of the [MG-RAST metagenomics analysis server](http://metagenomics.anl.gov). 
MG-RAST uses a centralized data server, so in the simulation, I look at adding proxy servers to help distribute the load of the data server, as well as a proxy-aware scheduling methodology that exploits the data locality provided by the proxy servers. 
This work was published at [PADS '16](http://www.acm-sigsim-pads.org/). 

Paper: [A Case Study in Using Discrete-Event Simulation to Improve the Scalability of MG-RAST](../papers/ross-pads16.pdf)

[Click here](../thesis/index.html) if you'd like to read more details on my dissertation.

I received an award from the [Department of Energy Office of Science Graduate Student Research program](https://science.energy.gov/wdts/scgsr/) to continue my thesis research at Argonne National Laboratory during Summer and Fall 2018.
[Here is RPI's article about my work and the award.](https://news.rpi.edu/content/2018/04/13/better-tools-supercomputer-research)


#### Data Science Intern, ViaSat, Carlsbad, CA

##### June 2017 - August 2017

Advisor: Chris Bishop </br>
Project: Anomaly Detection Service for Spark Streaming Data

The goal of this project was to develop a framework for finding anomalies in streaming data (e.g., finding network failures).
The anomaly detection framework was implemented in Scala and accepts Spark Streaming data of varying formats.
A few simple anomaly detection algorithms were implemented (e.g., exponential moving average), but the modular design of this framework allows for the easy addition of other anomaly detection algorithms.
To allow this service to be easily used by less technical employees, a web application was also developed which allows users to easily configure the anomaly detection service for their data without having to touch any of the code.
Anomaly detection results are written back to the data repository and ingested by a time series database, so results can be easily visualized using the Grafana dashboard visualization tool.

#### Intern, NASA Goddard Space Flight Center, Greenbelt, MD

##### June 2014 - August 2014

Advisor: Daniel Duffy<br/>
I worked for the NASA Center for Climate Simulation (NCCS).  While there, I worked with a Hadoop cluster that they used for storing climate data.  I evaluated the use of Impala and Hive with several file types (Sequence, RC, and Parquet).  Impala and Hive are both SQL query engines that run on Hadoop/HDFS, but Hive creates 1 or more MapReduce jobs from queries, whereas Impala uses massively parallel processing.  

#### Undergraduate Research Assistant, UNCG, Greensboro, NC

##### January 2012 - May 2014

Advisors: [Olav Rueppell](http://biology.uncg.edu/labs/rueppell/) and [Jan Rychtar](http://www.uncg.edu/mat/faculty/rychtar/) <br/>
In my first research project, I used game theory to develop a model to study the evolution of altruism.  We used Prisoner's Dilemma to determine the payoffs of interactions between cooperators and defectors.  In the model, individuals have biological ages (i.e. pre-reproductive, reproductive, and post-reproductive ages).  Individuals of reproductive age can reproduce with a probability proportional to their fitness relative to their neighbors.  I wrote a simulation in C++ that allowed us to vary parameters such as the benefit defectors receive from cooperators and average lengths of the age stages.

My second research project was a bioinformatics project.  We looked at the effect of genomic features on recombination rates in <i>Apis mellifera</i> (the honeybee).  Honeybees have very high recombination rates, even among social insects.  I wrote Python scripts to collect information about features, such as looking for certain motifs, di, tri, and tetra nucleotides, and so on. I also assisted a masters biology student with computational aspects of a related study.  
