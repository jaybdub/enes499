# nanopb_simple

In order to communicate between the Arduino and a host computer in a reliable, organized way, you may find Google's Protocol Buffers useful.  Google's Protocol Buffers allow you to define a message in a '.proto' file, and compile this message into C/C++ (or python, java, etc.) code that you can use in your programs.  

First let's get started with the installation.  

## Installation (Linux)

Here I assume you have Python2.7.X installed, if not download it [here]().

###Install Google Protocol Buffers
Download [protobuf-2.5.0.tar.gz](https://code.google.com/p/protobuf/downloads/list)

Extract the compressed file to a location of your choice (I chose /home/john/ A.K.A. ~/).  After extraction, in the terminal, change directories into ~/protobuf-2.5.0, configure, compile, and install.
	```
    cd ~/protobuf-2.5.0/
	./configure
	make
	make check
	sudo make install
	cd python
	python ./setup.py build
	sudo python ./setup.py install
	```
Okay, there you have it, protocol buffers have been installed.  To verify this type 

   protoc --version

If it responds with a message other than
	```
   libprotoc 2.5.0
	```
then try typing the following command
	```
	sudo ldconfig
	```

###Install nanopb

From their website, "Nanopb is a plain-C implementation of Google's Protocol Buffers data format. It is targeted at 32 bit microcontrollers, but is also fit for other embedded systems with tight (2-10 kB ROM, 1 kB RAM) memory constraints."

So basically, it's a version of Google's Protocol Buffers that you can use on your Arduino.  It is however, dependent on Protocol Buffers so the installation of Protocol Buffers was still necessary.

Assuming you have git installed type the following to download and compile nanopb.

    ```
	cd
	git clone https://code.google.com/p/nanopb
	cd ~/nanopb/generator/proto
	make
	```

