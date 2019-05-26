# Trader (CLI)
Latest Release: v1.0
Maintained by Team-COD.

## Information
Trader is a decentralized banking platform with encrypted messages and own privacy protected cryptocurrency.

Trader is based on the Cryptonote protocol and runs on a secure peer-to-peer network technology to operate with no central authority. You control your private keys to your funds, you control your destiny. Trader Network is accessible by anyone in the world regardless of his/her geographic location or status. Our blockchain is resistant to any kind of analysis. All your W2W transactions and messages are anonymous. Trader Network provides an instant secure, untraceable and unlinkable way of encrypted communication - crypto messages.

Trader is open-source, community driven and truly decentralized. No one owns it, everyone can take part.

## Resources
- Web: [Soon to come](Soon to come)
- GitHub: [https://github.com/zooteld/Trader.git](https://github.com/zooteld/Trader.git)
- Discord: [Soon to come](soon to come)
- Reddit: [Soon to come](Soon to come)
- Bitcoin Talk: [Soon to come](Soon to come)
- Paperwallet: [Soon to come](Soon to come)

## Compiling Trader from source

### Linux / Ubuntu

##### Prerequisites

- You will need the following dependencies to build the Trader CLI: boost, cmake, git, gcc, g++, python, and make.
- On Ubuntu: `sudo apt-get install -y build-essential python-dev gcc g++ git cmake libboost-all-dev`

#### Building

- `git clone https://github.com/zooteld/Trader.git
- `cd Trader`
- `mkdir build && cd $_`
- `cmake ..`
- `make`

If the build is successful the binaries will be in the src folder.

### Windows 10

##### Prerequisites

- Install [Visual Studio 2017 Community Edition](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15&page=inlineinstall)
- Install [CMake](https://cmake.org/download/)
- When installing Visual Studio, you need to install **Desktop development with C++** and the **VC++ v140 toolchain** components. The option to install the v140 toolchain can be found by expanding the "Desktop development with C++" node on the right. You will need this for the project to build correctly.
- Install [Boost 1.67.0](https://boost.teeks99.com/bin/1.67.0/), ensuring you download the installer for MSVC 14.1.

##### Building

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017' or run "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\Tools\VsMSBuildCmd.bat" from any command prompt.

- `git clone https://github.com/zooteld/Trader.git`
- `cd trader`
- `mkdir build`
- `cd build`
- `cmake -G "Visual Studio 15 2017 Win64" -DBOOST_LIBRARYDIR:PATH=c:/local/boost_1_67_0 ..` (Or your boost installed dir.)
- `msbuild concealX.sln /p:Configuration=Release /m`

If the build is successful the binaries will be in the src/Release folder.

### macOS

#### Prerequisites

In order to install prerequisites, [XCode](https://developer.apple.com/xcode/) and [Homebrew](https://brew.sh/) needs to be installed.
Once both are ready, open terminal app, run following command:

```bash
$ xcode-select --install
```

and install all tools. On newer macOS versions (v10.14 and higher) this step is done through Software Update app.

After that, proceed with installing dependencies:

```bash
$ brew install git python cmake gcc boost
```

When all dependencies are installed, build Trader Core binaries:

```bash
$ git clone https://github.com/zooteld/Trader.git
$ cd trader
$ mkdir build && cd $_
$ cmake ..
$ make
```

If the build is successful the binaries will be located in `src` directory.

#### Special Thanks
Special thanks goes out to the developers from Cryptonote, Bytecoin, Monero, Forknote, TurtleCoin, and Masari.
