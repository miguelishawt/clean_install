# clean install

Two simple scripts to install a project that uses CMake (with the patterns I use).

# Usage

Installing the library that uses CMake:

    sh ./install.sh

Cleaning the temporary binaries and cache created by CMake:

    sh ./clean.sh

# NOTES

1. A `build` directory is assumed to be created before you use the `install.sh` script. If you wish, you can do so by using the `clean.sh` script.
2. The `install.sh` script requires a `BUILD_SHARED_LIBS` boolean variable within CMake's build system. 
3. Debug and Release builds are built and installed, for both shared and static binaries.
4. The `install.sh` script does not delete your CMake cache, thus if you wish to have specific settings for your own build, you may do so. To do this, you must leave the CMake cache within the `build` directory. 

# License

Copyright (C) 2013 Miguel Martin (miguel.martin7.5@hotmail.com)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
