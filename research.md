---
title: Research 
layout: page
permalink: /research/index.html
---
<style>
img { width: 50%; margin: 0 auto; display: block; }
</style>

![Profile Image]({{ site.url }}/{{ site.picture }})

# Research Experience, Internships, and Projects

### Graduate Research Assistant, RPI

#### August 2014 - Present

Advisor: [Chris Carothers](http://www.cs.rpi.edu/~chrisc/) <br/>
Thesis: Performance Analysis and Visualization of Extreme-Scale Parallel Discrete-Event Simulations <br />

I have developed an instrumentation layer for the [ROSS PDES framework](https://github.com/carothersc/ROSS) that can collect detailed data about the simulation engine and the model being simulated.
We use this data to create visualizations that help us better understand the behavior of the simulations and find performance bottlenecks.
Early work in this area has been published in [PMBS '16](http://www.dcs.warwick.ac.uk/pmbs/pmbs/PMBS/Welcome.html).
For the rest of my dissertation, I'll be working on developing a system that runs along side ROSS that has in situ analysis and visualizations capabilities. 
With the help of this analysis system, I'll also be analyzing several HPC network topology models that are provided by the [CODES](http://www.mcs.anl.gov/research/projects/codes/) framework built on top of ROSS.

Paper: [Visual Data-Analytics of Large-Scale Parallel Discrete-Event Simulations](../papers/ross-pmbs16.pdf)


In the past, I've worked on a model of the [MG-RAST metagenomics analysis server](http://metagenomics.anl.gov). 
MG-RAST uses a centralized data server, so in the simulation, I look at adding proxy servers to help distribute the load of the data server, as well as a proxy-aware scheduling methodology that exploits the data locality provided by the proxy servers. 
This work was published at [PADS '16](http://www.acm-sigsim-pads.org/). 

Paper: [A Case Study in Using Discrete-Event Simulation to Improve the Scalability of MG-RAST](../papers/ross-pads16.pdf)

### Data Science Intern, ViaSat

#### June 2017 - August 2017

More details soon.

### Intern, NASA Goddard Space Flight Center

#### June 2014 - August 2014

Advisor: Daniel Duffy<br/>
I worked for the NASA Center for Climate Simulation (NCCS).  While there, I worked with a Hadoop cluster that they used for storing climate data.  I evaluated the use of Impala and Hive with several file types (Sequence, RC, and Parquet).  Impala and Hive are both SQL query engines that run on Hadoop/HDFS, but Hive creates 1 or more MapReduce jobs from queries, whereas Impala uses massively parallel processing.  

### Undergraduate Research Assistant, UNCG

#### January 2012 - May 2014

Advisors: [Olav Rueppell](http://biology.uncg.edu/labs/rueppell/) and [Jan Rychtar](http://www.uncg.edu/mat/faculty/rychtar/) <br/>
In my first research project, I used game theory to develop a model to study the evolution of altruism.  We used Prisoner's Dilemma to determine the payoffs of interactions between cooperators and defectors.  In the model, individuals have biological ages (i.e. pre-reproductive, reproductive, and post-reproductive ages).  Individuals of reproductive age can reproduce with a probability proportional to their fitness relative to their neighbors.  I wrote a simulation in C++ that allowed us to vary parameters such as the benefit defectors receive from cooperators and average lengths of the age stages.

My second research project was a bioinformatics project.  We looked at the effect of genomic features on recombination rates in <i>Apis mellifera</i> (the honeybee).  Honeybees have very high recombination rates, even among social insects.  I wrote Python scripts to collect information about features, such as looking for certain motifs, di, tri, and tetra nucleotides, and so on. I also assisted a masters biology student with computational aspects of a related study.  
