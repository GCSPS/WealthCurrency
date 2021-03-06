# WealthCurrency
GCSPS/WealthCurrency OpenSource Code
---

GIGA Space is a platform for anonymous applications such as P2P exchange, on-chain shop, Lotto, Gamble, and Bets. WealthCurrencyCoin (WTC) is the general currency in GIGASpace. 

The ultimate aim of GIGA Space is to be the most private and anonymous platform of crypto-currency applications, the ultimate aim of WealthCurrencyCoin is to be the general currency of the WealthCurrency world.

## Features ##
- Untraceable payments
- Unlinkable transactions
- Blockchain analysis resistance
- Adaptive parameters
- Transaction remote release
- Tor network

This project is based on [CryptoNote](https://cryptonote.org/) technology.

## Specifications ##
- Algorithm: Wild Scrypt
- Block Time: 60 seconds
- Difficulty: Retarget each block
- Total Coins: 200 million WTC


## Building ##
### Unix and MacOS X

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.53(but don't use 1.54) or later. You may download them from:
http://gcc.gnu.org/
http://www.cmake.org/
http://www.boost.org/
Alternatively, it may be possible to install them using a package manager.

More detailed instructions for OS X (assume you’re using MacPorts (they’re, however, pretty self-explanatory and homebrew users shouldn't have troubles following it too):

* Install latest Xcode and command line tools (these are in fact MacPorts prerequisites)
* Install GCC 4.8 and toolchain selector tool: `sudo port install gcc48 gcc_select`
* Set GCC 4.8 as an active compiler toolchain: `sudo port select --set gcc mp-gcc48`
* Install latest Boost, CMake: `sudo port install boost cmake`

To build, change to a directory where this file is located, and run `make`. The resulting executables can be found in `build/release/src`.

**Advanced options**:

Parallel build: run `make -j<number of threads>` instead of just `make`.

Debug build: run `make build-debug`.

Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.

Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`. *Warning, this will change your enviroment variable, if you do not know what this is, don't do it.

### Windows

Dependencies: MSVC 2012 or later, CMake 2.8.6 or later, and Boost 1.53(but don't use 1.54) or later. You may download them from:
http://www.microsoft.com/
http://www.cmake.org/
http://www.boost.org/

To build, change to a directory where this file is located, and run this commands: 
```bash
 mkdir build
 cd build
 cmake -G "Visual Studio 11 Win64" ..
```

And then do Build.
