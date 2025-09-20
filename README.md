# tools-installation
📚 Day 0: Tools Installation
This document provides a summary of the installation process for the required tools for the SFAL-VSD project. It includes the system requirements and a record of the successful installation of each tool. The instructions are based on the provided guide.

💻 System Requirements
The following machine configuration is recommended for this project:


RAM: 6 GB 



HDD: 50 GB 


OS: Ubuntu 20.04+ 


CPU: 4vCPU 
<img width="1853" height="966" alt="Screenshot 2025-09-20 182243" src="https://github.com/user-attachments/assets/4cd22754-4217-4d88-be71-c6d62744349c" />

Note: The provided screenshot shows the virtual machine running Ubuntu 24.04, which meets the OS requirement .

🛠️ Tool Installation and Verification
Here are the tools installed for the project, with commands and verification screenshots.

# Yosys

Yosys is an open-source framework for Verilog RTL synthesis[cite: 12].

**Installation Steps:**

1.  Update the package list:
    ```bash
    sudo apt-get update
    ```
2.  Clone the Yosys repository:
    ```bash
    git clone https://github.com/YosysHQ/yosys.git
    ```
3.  Navigate into the directory:
    ```bash
    cd yosys
    ```
4.  Install required dependencies (if not already installed):
    ```bash
    sudo apt install make
    sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
    ```
5.  Configure for GCC:
    ```bash
    make config-gcc
    ```
6.  Build the program:
    ```bash
    make
    ```
7.  Install the program system-wide:
    ```bash
    sudo make install
    ```

**Verification:**

<img width="1030" height="642" alt="Screenshot 2025-09-20 172529" src="https://github.com/user-attachments/assets/d38ef575-a27c-4959-90aa-ef0248cf80fb" />
<img width="1022" height="221" alt="Screenshot 2025-09-20 172504" src="https://github.com/user-attachments/assets/bcdbf6ae-186f-45ba-9c9f-6a29df5c0627" />

The installation was successful as confirmed by the terminal output showing the version and license information. .

# Icarus Verilog (Iverilog)

Icarus Verilog is a Verilog compiler and simulator.

Installation Steps:

Update the package list
```bash
sudo apt-get update
```
Install Icarus Verilog
```bash
sudo apt-get install iverilog
```

Verification:

<img width="772" height="297" alt="Screenshot 2025-09-20 172932" src="https://github.com/user-attachments/assets/054be2b5-c957-4822-a0a3-594c8a499981" />
<img width="1276" height="948" alt="Screenshot 2025-09-20 172913" src="https://github.com/user-attachments/assets/3c9d6c08-bebc-4f90-a204-c379f5d3fa7c" />

The installation was successful, and running the iverilog command displays its usage instructions, indicating the tool is properly installed and accessible. .

# GTKWave
GTKWave is a waveform viewer used to display simulation results.

Installation Steps:

Update the package list: 
```bash
sudo apt-get update.
```
Install GTKWave: 
```bash
sudo apt install gtkwave.
```
Verification:
<img width="1784" height="636" alt="Screenshot 2025-09-20 173126" src="https://github.com/user-attachments/assets/7fe49c30-0f3c-40f4-b006-4b03ddc6c3b5" />

The tool was successfully installed, and launching it with the gtkwave command opens the GTKWave Analyzer. .

