** Google's Protobuf for C++/Java/Python **
This library is awesome, creates classes for a variety of languages.
You will need to follow a tutorial :
[cpp tutorial](https://developers.google.com/protocol-buffers/docs/cpptutorial)

Also Download and install the library:
[download ](https://developers.google.com/protocol-buffers/docs/downloads)

You can also download the protobuf library for any platform.

** git clone https://developers.google.com/protocol-buffers/docs/downloads **

You will need protobuf to compile this address book

After installing source follow the steps below

* cd protobuf
* ./autogen.sh
* ./configure
* make
* make check
* sudo make install

You will have to either edit and add a path to your new lib.
Default installation is under /usr/local/lib

Edit /etc/ld.so.conf
Add your  installation directory path:   /usr/local/lib
Run    'sudo ldconfig'

clone this package
Comes with a Makefile so to compile run :
$ make all
