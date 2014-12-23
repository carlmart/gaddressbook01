# Google's Protobuf  #


This library is awesome, creates classes for a variety of languages.

Easy to use code generator for C++ / Java / Python

addressbook.proto does the magic. With the following code

you run 'make' and new files get generated.

```cpp
syntax="proto2";  // required there is now a proto3
package tutorial;

message Person {
  required string name = 1;
  required int32 id = 2;        // Unique ID number for this person.
  optional string email = 3;

  enum PhoneType {
    MOBILE = 0;
    HOME = 1;
    WORK = 2;
  }

  message PhoneNumber {
    required string number = 1;
    optional PhoneType type = 2 [default = HOME];
  }

  repeated PhoneNumber phone = 4;
}

// Our address book file is just one of these.
message AddressBook {
  repeated Person person = 1;
}


```


Follow the tutorial below :

[cpp tutorial](https://developers.google.com/protocol-buffers/docs/cpptutorial)

Also Download and install the library:

[download ](https://developers.google.com/protocol-buffers/docs/downloads)

You can also download the protobuf library for any platform.

* git clone https://developers.google.com/protocol-buffers/docs/downloads *

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

Run  :

```bash
sudo ldconfig'
```

Comes with a Makefile so to compile run :
```bash
make all
```
