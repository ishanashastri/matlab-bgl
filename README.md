MatlabBGL
=========

A C library wrapping the Boost graph library and a Matlab wrapper for the 
Boost graph library. **Updated to be compatible with a 64-bit MacOS configuration and newer versions of MATLAB (tested on R2019b).**

Features
--------

* Wrappers around most of the Boost graph library
functions
* Copy-free implementations of many graph algorithms
on Matlab's native sparse matrix type.
* Works effeciently on huge problems

Synopsis
--------

[coming soon]

Notes
-------
To recompile the MEX files manually through the Boost Graph library, first download the library (https://www.boost.org/users/history/version_1_72_0.html). In `libmbgl/compile-macosx-intel-64-large.sh`, make sure to change the `BOOST_DIR` to the path where your download is located at. 

Next, from your computer terminal, run,

```console
[matlab_bgl] $ cd libmbgl
[matlab_bgl/libmbgl] $ sh compile-macosx-intel-64-large.sh
```

Finally, from your MATLAB terminal, run,

```console
>> cd matlab_bgl
>> cd private
>> compile.m
```

In theory, this should recompile your MEX files and allow you to use the Boost Graph Library as desired. 

License
-------

Matlab code: BSD
libmbgl code: GPLv2

Copyright David F. Gleich, 2006-2011

