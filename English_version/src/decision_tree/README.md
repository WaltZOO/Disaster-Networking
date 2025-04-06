# Decision Tree

## Operation  
This document is intended for disaster network installers working on a specific area and terrain.  
The nodes represent decision variables that help define the exact need according to the terrain.

The leaves of the tree indicate which instruction file to follow in order to install a network that guarantees the following specifications while adapting to the characteristics of the terrain:  
- Two endpoints can communicate in bad weather conditions  
- Two endpoints can communicate if a relay node goes down (redundancy)

## Usage  
The user of the tree starts at the root and, for each node, answers the question asked. The answer will lead them one level deeper in the tree until reaching a leaf.  
They open the corresponding instruction file (`src/decision_tree/consignes/`) and follow the instructions to install their network.

