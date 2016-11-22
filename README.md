# awesome-embedded [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of delightful Embedded Systems [libraries, RTOSes, packages,](#packages-libraries-and-rtoses) and [references](#resources)!

*Please read the [contribution guidelines](contributing.md) before contributing.*

# Table of Contents

<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Packages, Libraries and RTOSes](#packages-libraries-and-rtoses)
	- [Communication](#communication)
	- [RTOS](#rtos)

	- [Testing](#testing)
	- [Frameworks](#frameworks)
	- [Embedded Linux](#embedded-linux)
	- [Alternative Languages (Not C/C++)](#alternative-languages-not-cc)
		- [Rust](#rust)
		- [Elixir](#elixir)
		- [Ada and Spark](#ada-and-spark)
		- [Javascript](#javascript)
	- [STL](#stl)
- [Resources](#resources)
	- [Podcasts](#podcasts)
	- [Videos](#videos)
	- [Books](#books)
	- [Standards](#standards)
	- [Tools](#tools)
	- [Courses](#courses)
- [License](#license)

<!-- /TOC -->

## Packages, Libraries and RTOSes

### Communication

- [nanopb](https://koti.kapsi.fi/jpa/nanopb/) - Nanopb is a plain-C implementation of Google's Protocol Buffers data format. It is targeted at 32 bit microcontrollers, but is also fit for other embedded systems with tight (2-10 kB ROM, <1 kB RAM) memory constraints.
- [lwIP](http://savannah.nongnu.org/projects/lwip/) - lwIP is a small independent implementation of the TCP/IP protocol suite that has been initially developed by Adam Dunkels.
- [CanFestival](http://www.canfestival.org/) - CanFestival focuses on providing an ANSI-C platform independent CANOpen® stack that can be built as master or slave nodes on PCs, Real-time IPCs, and Microcontrollers. 
- [CANopenNode](https://github.com/CANopenNode/CANopenNode) - CANopenNode is written in ANSI C in object-oriented way. It runs on different microcontrollers, as standalone application or with RTOS

### RTOS

- [FreeRTOS](http://www.freertos.org/) - A free use Real Time Operating system which is widely used and supports a large number of platforms.
- [RTEMS](https://www.rtems.org/) - Real-Time Executive for Multiprocessor Systems or RTEMS is an open source Real Time Operating System (RTOS) that supports open standard application programming interfaces (API) such as POSIX. It is used in space flight, medical, networking and many more embedded devices using processor architectures including ARM, PowerPC, Intel, Blackfin, MIPS, Microblaze and more.
- [uC/os](https://www.micrium.com/rtos/kernels/) - µC/OS-II and µC/OS-III are preemptive, highly portable, and scalable real-time kernels. You can test them out for free, but you must pay to put them into a product.
- [Fuschia](https://github.com/fuchsia-mirror/magenta) - Magenta is the core platform that powers the Fuchsia OS. Magenta is composed of a microkernel (source in kernel/...) as well as a small set of userspace services, drivers, and libraries (source in system/...) necessary for the system to boot, talk to hardware, load userspace processes and run them, etc. Fuchsia builds a much larger OS on top of this foundation.
- [TI-RTOS](www.ti.com/tool/ti-rtos) - A real-time operating system for TI microcontrollers, It Includes TCP/IP and USB stacks, a FAT file system, and device drivers, Most of the TI-RTOS components are released under the BSD License.

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
- [embedd.rs](http://embed.rs/) - Articles about doing embedded on rust

#### Elixir
- [Nerves](http://nerves-project.org/) - Uses buildroot to deploy Elixir programs running on the Erlang VM to embedded linux boards

#### Ada and Spark

- [AdaCore](https://github.com/AdaCore) - Open source maintainer of Ada with a focus on embedded use.

#### Javascript

- [Tessel](https://tessel.io/) - A openWRT based embedded system which can run Javascript.
- [JerryScript](https://github.com/Samsung/jerryscript) - A JavaScript engine intended to run on a very constrained devices such as microcontrollers. Designed for the Internet of Things.

### STL

- [ETL](https://github.com/etlcpp/etl) - Embedded Template Library which offers compile time defined container sizes, full C++ 03 and partial C++ 11 compatibility, deterministic behaviour, additional components for the embedded domain, etc. 

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
- [uC/OS-III, The Real-Time Kernel by Jean J Labrosse](https://www.amazon.com/dp/0982337531/ref=pd_lpo_sbs_dp_ss_3?pf_rd_p=1944687682&pf_rd_s=lpo-top-stripe-1&pf_rd_t=201&pf_rd_i=1578201039&pf_rd_m=ATVPDKIKX0DER&pf_rd_r=SVE997FF9MNQ1VYEJCM1) - A book about the Micrium's uC/os III. It is a great resource on how RTOSes for embedded systems should work.
- [An Embedded Software Primer by David E. Simon](https://www.amazon.com/Embedded-Software-Primer-David-Simon/dp/020161569X) - An introduction to embedded systems, with a good explanation to Real-time operating systems(RTOS).

### Standards

- [Embedded C Coding Standards](http://www.barrgroup.com/Embedded-Systems/Books/Embedded-C-Coding-Standard) - Coding standards for embedded C from the Barr Group.

### Tools

- [PlatformIO](http://platformio.org/) - PlatformIO is an open source ecosystem for IoT development
Cross-platform build system. Continuous and IDE integration. Arduino and ARM mbed compatible
- [Energia](http://energia.nu) - Energia is an open-source electronics prototyping platform, it brings the Wiring and Arduino framework to the Texas Instruments MSP430 based LaunchPad, it includes an IDE that is based on Processing.

### Courses

- [edX Embedded Systems Course by University of Texas Austin](https://www.edx.org/course/embedded-systems-shape-world-utaustinx-ut-6-03x)
- [UNC Charlotte Embedded Systems Course](https://www.youtube.com/playlist?list=PLE4462C1C306E2EB2) 
 
## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Chris Woodall](http://cwoodall.com) has waived all copyright and related or neighboring rights to this work.
