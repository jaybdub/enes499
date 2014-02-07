enes499
=======

Files, programs, and project management for UMD's enes499 course.

## Install Arduino

### Linux

**Option A:** Install automatically in a standard location

    sudo apt-get update
    sudo apt-get install arduino arduino-core

**Option B:** Install in a non-standard location without using the ubuntu package

1.  Downloading arduino 1.0.5 from [here](http://arduino.cc/en/Main/Software).
2.  After downloading, extract the folder into the home directory for your main user (for example /home/john).  And try running the program.

        cd ~/arduino-1.0.5
        ./arduino

3.  If it does not run, you likely need to install the Java openjdk-7-jre;

        sudo apt-get install openjdk-7-jre

4.  Install the compiler and libraries

        sudo apt-get install gcc-avr avr-libc
5.  Add USB port permissions for user

        sudo usermod -aG dialout <myuser>


