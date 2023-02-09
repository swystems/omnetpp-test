# omnetpp-test

This repository provides a template simple network simulation for [OMNet++](https://omnetpp.org/). 
It serves as base for simple tests and exercises to gain familiarity with the software.

This repo corresponds to [section 4.2](https://docs.omnetpp.org/tutorials/tictoc/part4/#42-channels-and-inner-type-definitions) 
of the [OMNet++ TicToc tutorial](https://docs.omnetpp.org/tutorials/tictoc/) 
(aside from some small modifications).

While exercises do not necessarily require to go through the entire tutorial (they can
be done intuitively based on the code in this repository), it is advised to do so to
gain a deeper understanding of OMNet++ simulations.

## Exercise guidelines

A list of exercises can be found in this repository's issues. An exercise usually consists 
in making small modifications to the current simulation. Below you can find guidelines to 
run an exercise.

1. Install [OMNet++](https://omnetpp.org/), **use version >= 6.0**.
2. Fork this repository (with your personal/orgaisation github account)
3. Clone the forked repository
4. Make a branch named "issue-" followed by the issue number. E.g. `issue-4` correspond
to the exercise outlined in issue number four.
5. Run the exisiting simulation:
    - Open OMNet++
    - File -> "Open Projects From File System" -> Browse to the repository folder 
    -> Finish
    - Click on the Run icon. This should automatically create a run configuration*
    - A new window should open with some nodes. Click on "Run with full animation" to
    see the simulation in action. 
    - Play with the buttons on the top bar to control the execution
> *if you have some errors such as "module not found", try to change the "run configurations" 
executable to "other" = `omnetpp-test/omnetpp-test`. If compilation fails instead there might 
be something wrong with your installation. 
6. Explore the source files: `tictoc.ned` (on the source tab) contains the network 
layout, `txc.cc` contains the source code with functions defining the network
behaviour, `omnetpp.ini` contains the configuration file. You should care only about
the first 2 files. 
7. _Implement the exercise and re-run the simulation_ (make sure you are working in the 
exercise branch).
8. Once the exercise is complete, *commit your changes and make a Pull Request* to the master 
branch of the forked repository. *Describe what the newly implemented network does* in the pull 
request description. 
9. Send the link of the pull request to us. 

**Useful resources**: [simulation manual](https://doc.omnetpp.org/omnetpp/manual/) 
