# 🛠️ Tool Setup Manual

This document provides setup guidelines for the key tools required in the RISC-V Reference SoC Tapeout Program.

---

## 1.📋 System Requirements
Before proceeding, verify that your system satisfies the minimum specifications listed below:

i)💾 RAM: 6 GB

ii)💽 Disk Space: 50 GB HDD

iii)🧠 Processor: 4 vCPUs

iv)🐧 OS: Ubuntu 20.04 or newer

---

## 1. 🔧 Yosys – RTL Synthesis

As an open-source logic synthesis tool, Yosys generates gate-level netlists from Verilog RTL, enabling physical design.

```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys

# Install dependencies
sudo apt install make  # (if not already installed)
sudo apt-get install build-essential clang bison flex \
  libreadline-dev gawk tcl-dev libffi-dev git \
  graphviz xdot pkg-config python3 libboost-system-dev \
  libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Build and install
make config-gcc
make
sudo make install

```
<img width="800" height="600" alt="yosys" src="https://github.com/user-attachments/assets/00fb4c05-748e-4310-9251-556202fea5d9" />

## 2.💻 Iverilog

As an open-source Verilog compiler and simulator, Iverilog enables the design and verification of digital circuits.

```bash
sudo apt-get update
sudo apt-get install iverilog

```
<img width="800" height="600" alt="iverilog" src="https://github.com/user-attachments/assets/0300bb5c-da5d-48ff-b4f4-5a0aa43aa467" />

## 3. 📈 GTKWave – Waveform Viewer

GTKWave provides waveform visualization for digital signals, mainly from Verilog and VHDL, during post-simulation debugging.

```bash
sudo apt-get update
sudo apt install gtkwave

```

<img width="800" height="600" alt="gtkwave" src="https://github.com/user-attachments/assets/61306619-23e7-4257-82dc-d4521843df0b" />

## 4. ⚡ Ngspice – Circuit Simulator

The Ngspice tool is widely used for mixed-signal circuit simulation, supporting analysis of transient voltages, currents, noise, and small-signal performance.
To install, download it from: https://sourceforge.net/projects/ngspice/files/
 and unpack in a local directory using

 ```bash
tar -zxvf ngspice-37.tar.gz
cd ngspice-37
mkdir release
cd release
../configure --with-x --with-readline=yes --disable-debug
make
sudo make install

```

<img width="800" height="600" alt="ngspice" src="https://github.com/user-attachments/assets/e4234314-67f5-4bc8-aeb5-19c557eda21b" />

## 5. 🧱 Magic – VLSI Layout Tool

As a VLSI layout editor, Magic enables interactive physical design and includes built-in support for DRC and circuit extraction.

Start by installing the dependencies:

```bash
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev \
  libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev
```

Clone and build Magic:

```bash
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
sudo make install
```
<img width="800" height="600" alt="magic" src="https://github.com/user-attachments/assets/c644277e-17ca-444e-9665-6ec6b9157bcb" />

## 🧪 Tool Installation Verification

Execute the following commands to ensure the correct versions are installed:

```bash
git --version
docker --version
python3 --version
python3 -m pip --version
make --version
```
## 📝 Note

The installation process assumes a Debian-based Linux environment (for example, Ubuntu 20.04 and above).

Before every major installation step, run sudo apt-get update.

A terminal restart or session re-login might be necessary once system tools are installed.









