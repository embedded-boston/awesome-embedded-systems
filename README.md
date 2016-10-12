# awesome-embedded [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of delightful Embedded Systems [libraries, RTOSes, packages,](#packages-libraries-and-rtoses) and [references](#resources)!

*Please read the [contribution guidelines](contributing.md) before contributing.*

# Table of Contents

<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Packages, Libraries and RTOSes](#packages-libraries-and-rtoses)
	- [Communication](#communication)
	- [Testing](#testing)
	- [Frameworks](#frameworks)
	- [Embedded Linux](#embedded-linux)
	- [Alternative Languages (Not C/C++)](#alternative-languages-not-cc)
		- [Rust](#rust)
		- [Elixir](#elixir)
		- [Ada and Spark](#ada-and-spark)
		- [Javascript](#javascript)
- [Resources](#resources)
	- [Podcasts](#podcasts)
	- [Videos](#videos)
	- [Books](#books)
	- [Standards](#standards)
	- [Tools](#tools)
- [License](#license)

<!-- /TOC -->

## Packages, Libraries and RTOSes

### Communication

- [nanopb](https://koti.kapsi.fi/jpa/nanopb/) - Nanopb is a plain-C implementation of Google's Protocol Buffers data format. It is targeted at 32 bit microcontrollers, but is also fit for other embedded systems with tight (2-10 kB ROM, <1 kB RAM) memory constraints.

### Testing

- [CppUTest](https://cpputest.github.io/) - unit testing and mocking framework for C/C++ with a focus on working for embedded systems!
- [ceedling, unity and cmock](http://www.throwtheswitch.org/) - Unit testing, mocking and build framework written in C with ruby for generating and building.

### Frameworks

- [Arduino](https://www.arduino.cc/)
- [ARM mbed](https://www.mbed.com/en/) - The ARM mbed IoT Device Platform provides the operating system, cloud services, tools and developer ecosystem to make the creation and deployment of commercial, standards-based IoT solutions possible at scale.

### Embedded Linux

- [yocto](https://www.yoctoproject.org/) - Yecto is a tool for creating custom embedded linux systems
- [Buildroot](https://buildroot.org/) - Buildroot is a simple, efficient and easy-to-use tool to generate embedded Linux systems through cross-compilation.

### Alternative Languages (Not C/C++)

#### Rust
- [Zinc](https://zinc.rs/) - Bare-metal ARM stack for rust. Aimed at replacing CMSIS or mbed (currently defunct)
- [rust-embedded](https://github.com/rust-embedded/rfcs) - RFCs proposed by the Rust community for better embedded systems support.

#### Elixir
- [Nerves](http://nerves-project.org/) - Uses buildroot to deploy Elixir programs running on the Erlang VM to embedded linux boards

#### Ada and Spark

- [AdaCore](https://github.com/AdaCore) - Open source maintainer of Ada with a focus on embedded use.

#### Javascript

- [Tessel](https://tessel.io/) - A openWRT based embedded system which can run Javascript.

## Resources

### Podcasts

- [Embedded](http://embedded.fm/) - Elicia White and Christopher White interview makes, hackers and engineers who work on embedded systems
- [The Amp Hour](http://www.theamphour.com/)
- [Sparkgap](http://thesparkgap.net/)

### Videos

- [EEVBlog](https://www.eevblog.com/) - More on the electronics side, but David L. Jones tears apart embedded systems and electronic devices.

### Books

- [Making Embedded Systems by Elicia White](https://www.amazon.com/Making-Embedded-Systems-Patterns-Software/dp/1449302149) - Covers the basics of embedded systems architecture, design and patterns.
- [Test Driven Developmet for Embedded C by James Grenning](https://www.amazon.com/Driven-Development-Embedded-Pragmatic-Programmers/dp/193435662X/ref=asap_bc?ie=UTF8) - How to approach test driven development for embedded devices written in C.

### Standards

- [Embedded C Coding Standards](http://www.barrgroup.com/Embedded-Systems/Books/Embedded-C-Coding-Standard) - Coding standards for embedded C from the Barr Group.

### Tools

- [PlatformIO](http://platformio.org/) - PlatformIO is an open source ecosystem for IoT development
Cross-platform build system. Continuous and IDE integration. Arduino and ARM mbed compatible

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Sindre Sorhus](http://sindresorhus.com) has waived all copyright and related or neighboring rights to this work.
