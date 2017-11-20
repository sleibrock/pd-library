PureData Library
=====================

PureData Library is a collection of PureData code aimed at being as modular as possible and re-usable across many projects.

## Installation

Clone the project with Git and then add the project to your library settings in PureData.
```bash
git clone https://github.com/sleibrock/pd-library
```


## Library Goals Checklist

* Additive and Subtractive Synthesizer modules
* Frequency Modulation Synthesizer module
* Granular Synthesis modules (sample and signal versions)
* Delay effect module
* Flanger effect module
* Left/Right Panner module
* Metronome/Timer module
* Quantizer module (matches inputs to beats)
* VCF control filter
* Eight-step arpeggiator
* 4-signal audio mixer
* Oscilloscope modules (64, 128, 256, 1024 samples)
* Envelope modules (ADSR, ramps, etc)


## Guidelines

* Modules must have GUIs for ease of use in projects
* Modules must have appropriate amount of inlets to control it
* Modules must have appropriate amount of outlets for data, events and logging
* Avoid cross-dependencies in the library to avoid slow-downs as much as possible
* Modules must end in "~" to indicate it outputs a signal stream (ex. "synth.pd" should be "synth~.pd")
* Variables must start with "$0-" to make sure there are no overlaps in send/receive variables

