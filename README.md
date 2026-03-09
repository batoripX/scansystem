# scansystem v1.0.0

A single-file system monitor for Android 16 that shows exact numbers. No dependencies. No approximations. Just truth.

## Philosophy

- **Exact numbers only** - Reads directly from /proc and /sys
- **No dependencies** - One file, statically linked
- **Security first** - No unsafe operations, minimal privileges
- **Beautiful UI** - Clean, modern interface with real-time graphs
- **Small footprint** - ~150KB binary, minimal memory usage

## Features

- **Real-time CPU monitoring** - Exact usage, temperature, core count
- **Memory tracking** - Used, available, cached, swap (byte-accurate)
- **Battery stats** - Level, voltage, current, temperature
- **60-second history graphs** - Visualize trends
- **Touch friendly** - Works with Android touch input
- **Beautiful UI** - Clean cards, progress bars, and real-time updates

## Installation

```bash
# Download the single binary
curl -L -o scansystem https://github.com/scansystem/releases/latest/download/scansystem

# Make executable
chmod +x scansystem

# Run (may need root for framebuffer access)
./scansystem
# Clone





##
git clone https://github.com/scansystem/scansystem
cd scansystem

# Build (requires Android NDK or clang with C++20)
clang++ -std=c++20 -O3 -flto -static -pthread \
    -o scansystem scansystem.cpp

# Strip binary (optional, reduces size)
strip scansystem
