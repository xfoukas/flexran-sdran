# FlexRAN SD-RAN platform
A platform for Software-Defined Radio Access Networks. 

This is the original version of the code as it appeared in the paper published at ACM CoNEXT 2016:

https://dl.acm.org/citation.cfm?id=2999599

For a newer version of the FlexRAN code please check the Mosaic5G project:

http://mosaic-5g.io/flexran/

If you are using FlexRAN for scientific papers, academic lectures, project reports, or technical documents, please help us by adding a reference to:

```
Foukas, X., Nikaein, N., Kassem, M. M., Marina, M. K., & Kontovasilis, K. (2016, December). 
FlexRAN: A flexible and programmable platform for software-defined radio access networks. In 
Proceedings of the 12th International on Conference on emerging Networking EXperiments and 
Technologies (CoNEXT) (pp. 427-441). ACM.
```

FlexRAN is composed of two parts:

* The FlexRAN real-time master controller
* The FlexRAN agent running at the eNodeB

This repository is meant to act as a central point from where both the code of
the controller and the agent can be obtained. 

To obtain the code, simply clone this repository and from its main directory run
```
git submodule init
```

Then choose to load the appropriate submodule depending on the deployment node 
(agent or controller).

## FlexRAN real-time controller

For the FlexRAN controller simply run:
```
git submodule update --remote flexran-rtc
```
The source code of the controller will be cloned from the appropriate repository
and can be found in the **flexran-rtc** directory.

## FlexRAN agent
For the FlexRAN agent simply run:
```
git submodule update --remote flexran-agent
```
The source code of the agent will be cloned and can be found in the 
**flexran-agent** directory.

## FlexRAN installation and execution
For instructions about installing and running FlexRAN, please see the tutorials
in the wiki.
