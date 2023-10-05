# cFS-Ransomware-POCs
Proof of concepts for various ransomware attack vectors on Core Flight System space vehicles 

This repository linked from the IEEE Aerospace Conference 2024 paper, "Guarding the Galaxy: Satellite Ransomware and Countermeasures".

It provides code examples for the proof-of-concept ransomware vectors demonstrated in the paper, designed to illustrate potential vulnerabilities in NASA's open source Core Flight System (cFS) architecture for research purposes. Note that none of these attack vectors exfiltrate data to outside sources or have been tested on cube satellite hardware - only simulated virtual instances as proof-of-concept demonstrations.

As these vectors are written specifically for cFS v6.7.0a, they are not guaranteed to work with future versions. Each vector contains modified files that are bundled with cFS as part of the architecture. To implement one, please [download and setup a virtual instance of cFS](https://github.com/nasa/cFS), then follow the instructions in each folder to place the files in their approriate locations in the file structure.

You may need to recompile the cFS framework with the following commands, providing a password as required:

```
cd /home/nos3/OpenSatKit-master/cfs`
sudo make install
```

After recompilation, the following commands will launch the cFS interface with modified components for testing:

```
cd /home/nos3/OpenSatKit-master/cosmos
ruby Launcher
```
