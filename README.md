** Google's Protobuf for C++/Java/Python **
This library is awesome, creates classes for a variety of languages
[cpp tutorial](https://developers.google.com/protocol-buffers/docs/cpptutorial)
[download protobuff lib](https://developers.google.com/protocol-buffers/docs/downloads)

You can also download the protobuf library for any platform.
I used it on Linux .
git clone https://developers.google.com/protocol-buffers/docs/downloads

You will need protobuf to compile 
After installing source
* cd protobuf
* ./autogen.sh
* ./configure
* make
* make check
* sudo make install

You will have to either edit and add a path to your new lib
default installation is under /usr/local/lib

Edit /etc/ld.so.conf
add installation directory /usr/local/lib
sudo ldconfig

clone this package
Comes with a Makefile so to compile run :
$ make all
