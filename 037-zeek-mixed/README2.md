# 037-zeek-mixed

# Description
Benign windows computer doing normal activities, attacked form the Internet.

## Origin
This capture is the complete (24hs) first day (Day1) of a capture that was originally named `CTU-Normal-45`.

## Author
The capture was done in the Stratosphere Laboratory, Czech Technical University in Prague, Czech Republic as part of the master [thesis](https://dspace.cvut.cz/bitstream/handle/10467/107647/F3-DP-2023-Janata-Pavel-Master_Thesis_Pavel_Janata.pdf?sequence=-1&isAllowed=y) of Pavel Janata for the [FEEL project](https://github.com/stratosphereips/feel_project) about federated learning.


## Format
Zeek logs

## IPs
- Benign host: 147.32.85.12

## Labels
The capture was supposedly only benign when it was done, but the computer was connected to the Internet so it was attacked. Therefore we label all those attacks correctly.

The labels are assigned per-flow following the rules described in the file `labels.config` and the program [NetflowLabeler](https://github.com/stratosphereips/netflowlabeler).

