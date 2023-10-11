# cFS-Ransomware-POCs
This repository linked from the IEEE Aerospace Conference 2024 paper, "Guarding the Galaxy: Satellite Ransomware and Countermeasures".

It provides a code example for the proof-of-concept ransomware vector demonstrated in the paper, designed to illustrate potential vulnerabilities in NASA's open source Core Flight System (cFS) architecture for research purposes. Note that this attack vector does not exfiltrate data to outside source and has not been tested on cube satellite hardware - only simulated virtual instances as a proof-of-concept demonstration.

As this vector is written specifically for cFS v6.7.0a, it is not guaranteed to work with future versions. The attack contains modified files that are bundled with cFS as part of the architecture. To implement, please [download and setup a virtual instance of cFS](https://github.com/nasa/cFS), then follow the steps in _Instructions.md_ to place the files in their approriate locations within the file structure.

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
