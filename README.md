# Quick learning project
This hackathon side project was y intro to SQL and IPyWidgets with Jupyter Notebook for dynamic data vizualization

## hwt-Fall23
HACKWESTX Fall 2024 Challenge Problems

<img src="https://www.hackwestx.tech/_next/static/media/screen.7094e3a8.svg" alt="HACKWESTX Logo" width="50"/>


## Overview

The Structural Simulation Toolkit (SST) is a parallel discrete event
simulation infrastructure designed to support multi-reslution simulations.
In this case, SST is most often utilized to simulate a variety of different
computer architecture devices/components.  Unlike other simulation infrastructures
such as QEMU and Gem5, SST utilizes MPI (message passing interface) and C++ threading
such that simulations can be scaled out to a large number of host systems.  This
permits us to build full-system simulations with high fidelity components
for each discrete architectural unit.

One of the inherent downsides to building very large simulation experiments
is the size and scope of the output data can be very large.  SST provides
distinct statistics output from each unique SST component in a variety of
forms (CSV being the most common).  For this challenge problem, we seek
to ingest these large, structured CSV files into a web-based, graphical
visualization and analysis infrastructure written in Python.  We are providing 
SQLite3 database files that includes sample statistics output from sample 
simulations.

The difficulty in ingesting these data files into SST is that the particular
components and included data will not be known until the filese are actually
ingested.  Further, we seek to cross correlate events and data values across
disparate component data units in the visualization tool.

Be creative!  Dynamic visualizations will be given priority over basic, static
graphs.  Additional points will be given to those that can build, run and demonstrate
SST, especially if you can stream data directly into the visualization tool.

## Requirements

There are a number of basic requirements for this challenge, including:
* You must ingest and build the visualizations from the provided files.  Note
that you *CANNOT* build visualization templates beforehand.  They must be
generated dynamically.
* You *MUST* have a file selection utility so you can select different SQLite3 
database files
* You *MUST* be able to select different graph types and different statistics 
from the target database input file.  EG, `SELECT stat1,stat2 from database` from 
a user input
* Any external plugins utilized must be MIT, BSD or Apache licensed.  No GPL-3 code
will be accepted
* Jupyter notebooks tools/libraries CAN be used!

## Deliverables

The deliverables for this challenge include:
* A working demo of your integrated visualization infrastructure.  We must see it work!
* Any source code associated with the solution (scripts, etc)
* Concise documentation to build, integrate and test the solution.  This should also
include any required external packages outside of what is outlined above.

## Licensing

See the top-level LICENSE file

## Contact
* *John Leidel* - *Chief Scientist* - [Tactical Computing Labs](http://www.tactcomplabs.com)

