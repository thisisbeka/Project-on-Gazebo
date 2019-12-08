## Installation

To install Gazebo follow [official web page](http://gazebosim.org/tutorials?cat=install) instructions.

### Ubuntu - Linux

```bash
sudo apt-get install gazebo9 libgazebo9-dev
```

### Mac OS

```bash
brew tap osrf/simulation
brew install gazebo9
```
## Build *sitl_gazebo*

Clone the repository to your computer.

**IMPORTANT: If you do not clone to ~/src/sitl_gazebo, all remaining paths in these instructions will need to be adjusted.**

```bash
mkdir -p ~/src
cd src
git clone --recursive https://github.com/PX4/sitl_gazebo.git
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
