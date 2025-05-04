# 008-zeek-mixed

## Description
This capture is the first day (24hs) of a capture that was originally named `CTU-Normal-40` and was part of the group of captures of the `CTU-50` dataset that was published separatedly.
The capture was done as part of the master [thesis](https://dspace.cvut.cz/bitstream/handle/10467/107647/F3-DP-2023-Janata-Pavel-Master_Thesis_Pavel_Janata.pdf?sequence=-1&isAllowed=y) of Pavel Janata for the [FEEL project](https://github.com/stratosphereips/feel_project) about federated learning.

It was done in the Stratosphere Laboratory, Czech Technical University in Prague, Czech Republic.

There are six more days that are included separatedly in this repository.

# Format
Zeek logs

## Labels
The capture was supposedly only benign when it was done, but the computer was connected to the Internet so it was attacked. Therefore we label all those attacks correctly.

The labels are assigned per-flow following the rules described in the file `labels.config` and the program [NetflowLabeler](https://github.com/stratosphereips/netflowlabeler).

