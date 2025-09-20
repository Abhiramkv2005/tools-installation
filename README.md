# tools-installation
📚 Day 0: Tools Installation
This document provides a summary of the installation process for the required tools for the SFAL-VSD project. It includes the system requirements and a record of the successful installation of each tool. The instructions are based on the provided guide.

💻 System Requirements
The following machine configuration is recommended for this project:


RAM: 6 GB 


HDD: 50 GB 


OS: Ubuntu 20.04+ 


CPU: 4vCPU 

Note: The provided screenshot shows the virtual machine running Ubuntu 24.04, which meets the OS requirement .

🛠️ Tool Installation and Verification
Here are the tools installed for the project, with commands and verification screenshots.

Yosys
Yosys is an open-source framework for Verilog RTL synthesis.

Installation Steps:

Update the package list: 

sudo apt-get update.

Clone the Yosys repository: 

git clone https://github.com/YosysHQ/yosys.git.

Navigate into the directory: 

cd yosys.

Install required dependencies: 

sudo apt install make, followed by sudo apt-get install build-essential clang bison flex libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev.

Configure for GCC: 

make config-gcc.

Build the program: 

make.

Install the program system-wide: 

sudo make install.

Verification:

The installation was successful as confirmed by the terminal output showing the version and license information. .

Icarus Verilog (Iverilog)
Icarus Verilog is a Verilog compiler and simulator.

Installation Steps:

Update the package list: 

sudo apt-get update.

Install Icarus Verilog: 

sudo apt-get install iverilog.

Verification:

The installation was successful, and running the iverilog command displays its usage instructions, indicating the tool is properly installed and accessible. .

GTKWave
GTKWave is a waveform viewer used to display simulation results.

Installation Steps:

Update the package list: 

sudo apt-get update.

Install GTKWave: 

sudo apt install gtkwave.

Verification:

The tool was successfully installed, and launching it with the gtkwave command opens the GTKWave Analyzer. .

ngspice
ngspice is a circuit simulator.

Installation Steps:

Download the ngspice tarball.

Unpack the tarball: 

tar -zxvf ngspice-37.tar.gz.

Navigate to the directory: 

cd ngspice-37.

Create a release directory: 

mkdir release.

Navigate into the release directory: 

cd release.

Configure the build: 

../configure --with-x --with-readline yes --disable-debug.

Build the program: 

make.

Install the program system-wide: 

sudo make install.

Verification:

Running ngspice -v shows the version and copyright information, confirming the installation was successful. .

Magic VLSI Layout Tool
Magic is a VLSI layout tool.

Installation Steps:

Install dependencies: 

sudo apt-get install m4, tcsh, csh, libx11-dev, tcl-dev tk-dev, libcairo2-dev, mesa-common-dev libglu1-mesa-dev, and libncurses-dev.

Clone the repository: 

git clone https://github.com/RTimothyEdwards/magic.

Navigate into the directory: 

cd magic.

Configure the build: 

./configure.

Build the program: 

make.

Install the program: 

make install.

Verification:

The installation was successful. The magic command opens the Magic VLSI layout tool GUI, and the terminal output confirms the tool is running. .
