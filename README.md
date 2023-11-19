# Bus-Routing



## Description
the project was developed to address the bus route problem in cities, such as delays, vacant buses, and so on

the idea is to create a graph in which its nodes are the bus stops and edges are the roads between the bus stops

then each node is given a value between 0-20 in jumps of 5 which resembles the passengers waiting at the bus stop

which will later on be used to give a certain weight to the edges, The Euclidean distance is also calculated between nodes

then Dijkstra algorithm is used on random pairs of nodes to find the shortest path between them

we then train the model using these paths each node data in the path is augmented which will be our train features and the node itself will be the label

we will train the model by giving him the starting node of the path and finding the next nodes in the same order as the Dijkstra path




## Table of Contents


  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Running the code](#running-the-code)
  


## Features

Machine learning approach to solve the problem

Dijkstra algorithm

Networkx to build the graphs

MXNET model for training

Python



## Getting Started



### Prerequisites

Networkx 

Apache MXnet

Numpy

Tensorflow

Anvil

Matplotlib

These packages must be installed prior to starting, the user must make sure the package versions support the other packages.


### Running the code

Training the model & statistics:

For training the model from the start, the user must run the code in Training-Bus_Router.ipynb we provided on Google Colab, a few changes must be made:

1. The user must connect to their own Google Drive account

2. The user must change the paths to their own Google Drive account to save and load the model parameters

After those changes are done, the user now can run all the cells either by choosing runtime->run all from the nav bar of Google Collab, or by running each cell one by one.

Once all the cells finish running the user can see the results in the output box under each cell.
 



Using the model:

After training the model at least once, now we should have the model parameters saved in our Google Drive, the user can now run the cells without the cells containing the model training and results/tests.







Using anvil server:

After running all the cells, the last cell is used for the Anvil server, once it's running it runs forever (or until the Google Collab runtime is disconnected)

once this cell is running the user can head to the public URL to use the Anvil interface, the user can 

calculate 5 routes of their choice, the source and destination must be numbers between 0-49, once the user fills the five routes' source and destination fields 

he then can click calculate Routes to see the resulting routes when clicking the route# button the route # is

shown, the user can click back in order to calculate 5 different routes








