# clean install

Two simple scripts to install a project that uses CMake (with the patterns I use).

# Usage

Installing the library that uses CMake:

    ./install.sh

Cleaning the temporary binaries and cache created by CMake:

    ./clean.sh

# NOTES

1. A `build` directory is assumed to be created before you use the `install.sh` script. If you wish, you can do so by using the `clean.sh` script. Alternatively,
   you can pass your own directory to the script to where it should store temporary CMake files
   (e.g. `./install.sh .`), but I reccomend using a build directory to keep the root directory clean.
2. The `install.sh` script requires a `BUILD_SHARED_LIBS` boolean variable within CMake's build system. 
3. Debug and Release builds are built and installed, for both shared and static binaries.
4. The `install.sh` script does not delete your CMake cache, thus if you wish to have specific settings for your own build, you may do so. To do this, you must leave the CMake cache within the `build` directory. 

# License

See [LICENSE](LICENSE).
