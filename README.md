## SIMH-v3.12
### The Computer History Simulation Project 
---

### This repository contains the SIMH v3.12 releases from Bob Supnik's web site.

You are highly encouraged to visit https://simh.trailing-edge.com as there is trove of useful information and code there.  

Each version is contained in its own subdirectory. They are expanded versions of the zip files from the trailing-edge web site.

Each release is downloaded here to allow you to fork / clone for your own personal development.  
No attempt has been made (yet) to make each version a series of commits to show what has changed between versions.

---

### From the current simh.trailing-edge.com site:


#### Computer Simulation and History

This site (https://simh.trailing-edge.com) documents SimH, a simulator for historic computer 
systems, as well as papers and reflections on the history of computing.

SimH (History Simulator) is a collection of simulators for historically significant 
or just plain interesting computer hardware and software from the past. The goal of the project 
is to create highly portable system simulators and to publish them as open-source 
software on the Internet, with freely available copies of significant or representative software.

This site contains the "classic" version of SimH, the 3.X stream. It includes all of the 
simulators I wrote or maintain, as well as the current releases of J. David Bryan's HP simulators. 
It also has a collection of papers and software kits that are applicable to all versions of SimH.

The V4 stream is substantially enhanced and contains many additional simulators. 
It can be found on GitHub under the name Open-SimH.

The source code in both V3 and (Open SimH) V4 is licensed under an "MIT-style" open-source license. 
Contributions to either stream are welcome if (and only if) they include this style of open-source license.
It
#### Simulators

SIMH is a highly portable, multi-system simulator.

-    Download the latest sources and documentation for SIMH V3.12-5, updated 16-Jul-2024.   
     Older releases can be found [here](https://simh.trailing-edge.com/sources/archive/ "Archive").
    
-    Download the latest sources, documentation, and software kits for Dave Bryan's [HP simulators](https://simh.trailing-edge.com/hp/ "HP Simulators").
    
-    Download PDF copies of the documentation [here](https://simh.trailing-edge.com/pdf/all_docs.html "Documentation").


SIMH V3.x implements simulators for:

-    Data General Nova, Eclipse
-    Digital Equipment Corporation PDP-1, PDP-4, PDP-7, PDP-8, PDP-9, PDP-10 (KS10), PDP-11, PDP-15 (and UC15), VAX11/780, VAX3900
-    GRI Corporation GRI-909, GRI-99
-    IBM 1401, 1620, 7090/7094, System 3
-    Interdata (Perkin-Elmer) 16b and 32b systems
-    Hewlett-Packard 2114, 2115, 2116, 2100, 21MX, 1000, 3000
-    Honeywell H316/H516
-    MITS Altair 8800, 8080 only
-    Royal-McBee LGP-30, LGP-21
-    Scientific Data https://simh.trailing-edge.com/sources/simtools/Systems SDS 940
-    Xerox Data Systems Sigma 32b systems 

Also available are a collection of [tools](https://simh.trailing-edge.com/sources/simtools/ "SimTools") for manipulating simulator file formats and for cross-assembling code for the PDP-1, PDP-7, PDP-8, and PDP-11. 


#### Release Notes for V3.12-5

Released 16-Jul-2024:

This release is mostly bug fixes, particularly in the PDP-11 and Sigma simulators. 
Chaosnet support has been added to the PDP-10 and PDP-11. 
See the detailed revision histories in individual source code modules for details. 

#### Release Notes for V3.12-4

Released 2023-06-05:

[Editors note:  Sorry, I didn't retrieve the Release notes for this version]

#### Release Notes for V3.12-3

Released 2022-12-16:

This release is mostly bug fixes, particularly in the PDP-11 and Sigma simulators. 
Support for running SimH on MacOS "Classic" (pre-OSX) and OS/2 has been dropped. 
See the detailed revision histories in individual source code modules for details. 

#### Release Notes for V3.12-2

Released 2022-04-26:

This is the first official release of SimH 3.X in more than two years. 
It includes numerous bug fixes and extensions to the individual simulators, as well as a few major upgrades in capability:

-    The magtape library (sim_tape.c) has been extended to allow the inclusion of private metadata in SimH format tapes. The extension is backward compatible to the previous format and is invisible to simulators that do not need or support private metadata.
-    To support the tape format extension, there is a new version of the mtdump utility. In addition to supporting the extended SimH tape format, it supports P7B (Pierce 7bit) format for the first time.
-    Support for non-standard C compliant compilers has been dropped. 

See the detailed revision history in *sim_rev.h* for more details. 
