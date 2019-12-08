## Installation

To install Gazebo follow [official web page](http://gazebosim.org/tutorials?cat=install) instructions.

### Ubuntu - Linux

```bash
sudo apt-get install gazebo9 
```

### Mac OS

```bash
brew tap osrf/simulation
brew install gazebo9
```
## Build *sitl_gazebo*

Now, clone the repository to your device:

```bash
mkdir -p ~/src
cd src
git clone --recursive https://github.com/thisisbeka/Project-on-Gazebo
```

Create a build folder in the top level of your repository:

```bash
mkdir build
```

Navigate into the build directory and invoke CMake from it:

```bash
cd ~/src/sitl_gazebo
cd build
cmake ..
```

Now build the gazebo plugins by typing:

```bash
make -j$(nproc) -l$(nproc)
```
## License
[MIT](https://choosealicense.com/licenses/mit/)
