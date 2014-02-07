enes499
=======

Files, programs, and project management for UMD's enes499 course.

## Install Arduino

### Linux

To install in a non-standard location without using the ubuntu package, begin by downloading arduino 1.0.5 from [here](http://arduino.cc/en/Main/Software).
After downloading, extract the folder into the home directory for your main user (for example /home/john).

To run:

    cd ~/arduino-1.0.5
    ./arduino

If it does not run, you likely need to install the Java openjdk-7-jre;

    sudo apt-get install openjdk-7-jre

To install automatically in a standard location:

    sudo apt-get update
    sudo apt-get install arduino arduino-core
