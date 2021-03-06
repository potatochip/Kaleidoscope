# Getting Started

## Setup the Arduino IDE

Setup the Arduino IDE on your system. Make sure you install at least version 1.8.6, since older version may not support all required features.

* On Linux, follow the instructions [on the wiki](https://github.com/keyboardio/Kaleidoscope/wiki/Install-Arduino-support-on-Linux).
* On macOS, install using [homebrew](http://brew.sh/) [cask](https://caskroom.github.io/) with `brew cask install arduino` or download the application from [the official website](https://www.arduino.cc/en/Main/Software) and move it to your `/Applications` folder.

## Get into the right directory

### macOS
```sh
mkdir -p $HOME/Documents/Arduino/hardware
cd $HOME/Documents/Arduino/hardware
```

### Linux

```sh
mkdir -p $HOME/Arduino/hardware
cd $HOME/Arduino/hardware
```

### Windows

*TODO*: Write me

### Install the libraries and hardware definitions

## Clone the hardware definitions
```sh
git clone --recursive https://github.com/keyboardio/Kaleidoscope-Bundle-Keyboardio.git keyboardio

```

## Build the Kaleidoscope Firmware for your keyboard

(This part assumes you're building firmware for the Keyboardio Model 01)

```sh
# Go to your device firmware directory
cd keyboardio/avr/libraries/Model01-Firmware

# Build your firmware!
make


# Install your firmware
make flash
