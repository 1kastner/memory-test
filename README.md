# memory-test
Implementation of a Sternberg task with a free library and a helpful docker setup.
This project is meant as a possible template of how to easily setup an experiment and share it.

# jspsych
As you can see this project has https://github.com/jspsych/jsPsych as a submodule.
At the time of writing no npm or bower package is available, therefore this seems to be the easiest solution.
Please have a look at the project yourself regarding license issues, accredition etc.

To make git write the jsPsych code to the hard drive, the submodule must be explicitely initialised and updated, i.e.
```
git submodule init 
git submodule update
```


# the docker / couchdb setup
I wanted to provide a simple solution for saving the data from the experiment.
Within the jsPsych project at the time of writing there are some solution sketches but no server included.
I wanted to provide a simple solution to start with with docker.
That helps you not to clutter your environment with software you don't need and lateron can't remove properly.
Attention: There are no security measurements whatsoever and they are not planned to be introduced. 
This is a simple template to start with.
Use at your own dangeour.
For more information see the [License](LICENSE).
