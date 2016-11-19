# Xataface Documentation

This project includes documentation for [Xataface](http://xataface.com).  PHP API docs are generated using [Doxygen](http://www.stack.nl/~dimitri/doxygen/), 
while Javascript docs are generated using [JSdoc](http://usejsdoc.org/), which is bundled in the build_tools directory.

There is also a directory containing some documentation in markdown format in the markdown-docs directory.  This documentation will eventually
be moved to the [Xataface Wiki](https://github.com/shannah/xataface/wiki) on GitHub.

## Generating the Docs

### Requirements

1. Java 1.7 or higher
2. ANT 1.8 or higher
3. Doxygen 1.7 or higher

This project includes a build.xml file with some key tasks:

~~~~
$ ant -p
Buildfile: /Applications/XAMPP/xamppfiles/htdocs/xataface-docs/build.xml

Main targets:

 all      Generate All Documentation
 doxygen  Generate Doxygen Docs
 jsdoc    Generate jsdoc documentation
Default target: all
~~~~

To build all docs, simply run:

~~~~
$ ant
~~~~

NOTE:  You will likely need to provide the path to doxygen as follows:

~~~~
$ ant -Ddoxygen=/path/to/doxygen
~~~~

The hard-coded path in the build file points to the location on my build machine.

Docs will be generated inside the build directory.