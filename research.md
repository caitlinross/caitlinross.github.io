---
title: Research 
layout: page
permalink: /research/index.html
---
<style>
img { width: 50%; margin: 0 auto; display: block; }
</style>

![Profile Image]({{ site.url }}/{{ site.picture }})

<h1>Research Experience, Internships, and Projects</h1>
<h3>Graduate Research Assistant, RPI</h3>
<h4>August 2014 - Present</h4>
<p>Advisor: <a href="http://www.cs.rpi.edu/~chrisc/">Chris Carothers</a><br/>
I work in the area of parallel discrete-event simulation (PDES).  Currently I am working on adding support for performance analysis and visualization to the <a href="https://github.com/carothersc/ROSS">ROSS</a>  and <a href="http://www.mcs.anl.gov/research/projects/codes/">CODES</a> optimistic PDES frameworks.  Specifically I am adding instrumentation capabilities to ROSS to collect data about the simulation engine so we can understand how the performance is affected by the rollback behavior of different models.  </p>

<p>
In the past, I've worked on a model of the <a href="http://metagenomics.anl.gov">MG-RAST metagenomics analysis server</a>. MG-RAST uses a centralized data server, so in the simulation, I look at adding proxy servers to help distribute the load of the data server, as well as a proxy-aware scheduling methodology that helps to reduce data movement over wide area network links.  This work was published in <a href="http://www.acm-sigsim-pads.org/">PADS '16</a>. You can find the paper <a href="http://www.mcs.anl.gov/publication/case-study-using-discrete-event-simulation-improve-scalability-mg-rast">here</a>. 
</p>
<h3>Intern, NASA Goddard Space Flight Center</h3>
<h4>June 2014 - August 2014</h4>
<p>Advisor: Daniel Duffy<br/>
I worked for the NASA Center for Climate Simulation (NCCS).  While there, I worked with a Hadoop cluster that they used for storing climate data.  I evaluated the use of Impala and Hive with several file types (Sequence, RC, and Parquet).  Impala and Hive are both SQL query engines that run on Hadoop/HDFS, but Hive creates 1 or more MapReduce jobs from queries, whereas Impala uses massively parallel processing.  
</p>
<h3>Undergraduate Research Assistant, UNCG</h3>
<h4>January 2012 - May 2014</h4>
<p>Advisors: <a href="http://biology.uncg.edu/faculty/olav_rueppell/">Olav Rueppell</a> and <a href="http://www.uncg.edu/mat/faculty/rychtar/">Jan Rychtar</a><br/>
In my first research project, I used game theory to develop a model to study the evolution of altruism.  We used Prisoner's Dilemma to determine the payoffs of interactions between cooperators and defectors.  In the model, individuals have biological ages (i.e. pre-reproductive, reproductive, and post-reproductive ages).  Individuals of reproductive age can reproduce with a probability proportional to their fitness relative to their neighbors.  I wrote a simulation in C++ that allowed us to vary parameters such as the benefit defectors receive from cooperators and average lengths of the age stages.
</p>
<p> My second research project was a bioinformatics project.  We looked at the effect of genomic features on recombination rates in <i>Apis mellifera</i> (the honeybee).  Honeybees have very high recombination rates, even among social insects.  I wrote Python scripts to collect information about features, such as looking for certain motifs, di, tri, and tetra nucleotides, and so on. I also assisted a masters biology student with computational aspects of a related study.  
</p>
