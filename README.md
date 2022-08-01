# awesome-embedded [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of delightful Embedded Systems [libraries, RTOSes, packages,](#packages-libraries-and-rtoses) and [references](#resources)!

*Please read the [contribution guidelines](contributing.md) before contributing.*

# Table of Contents

<!-- TOC depthFrom:2 depthTo:6 orderedList:false updateOnSave:false withLinks:true -->

- [Packages, Libraries and RTOSes](#packages-libraries-and-rtoses)
    - [TCP/IP](#tcpip)
    - [CoAP](#coap)
    - [CANopen](#canopen)
        - [Open Source](#open-source)
        - [Proprietary](#proprietary)
    - [Serialization](#serialization)
    - [RTOS](#rtos)
        - [Free or Open Source](#free-or-open-source)
        - [Commercial](#commercial)
    - [Testing](#testing)
    - [Frameworks](#frameworks)
    - [Alternative Languages (Not C/C++)](#alternative-languages-not-cc)
        - [D](#d)
        - [Rust](#rust)
        - [Elixir](#elixir)
        - [Ada and Spark](#ada-and-spark)
        - [Javascript](#javascript)
        - [Nim](#nim-lang)
        - [Zig](#zig-lang)
        - [Clojure](#clojure)
        - [Golang](#golang)
    - [STL](#stl)
- [Resources](#resources)
    - [Other Lists](#other-lists)
    - [Podcasts](#podcasts)
    - [Videos](#videos)
    - [Books](#books)
    - [Standards](#standards)
    - [Tools](#tools)
    - [Embedded Linux](#embedded-linux)
    - [Courses](#courses)
- [License](#license)

<!-- /TOC -->

## Packages, Libraries and RTOSes

### TCP/IP

- [lwIP](http://savannah.nongnu.org/projects/lwip/) - lwIP is a small independent implementation of the TCP/IP protocol suite that has been initially developed by Adam Dunkels. Supports DHCP with AutoIP fallback, UDP, TCP, and an interrupt driven model.
- [uIP](https://github.com/adamdunkels/uip) - A very tiny IP stack, but also a very minimal IP stack. (Not maintained anymore)

### CoAP

- [cantcoap](https://github.com/staropram/cantcoap) - Small and lightweight coap encoder and decoder. Protocol level stuff is left to the user.
- [libcoap](https://libcoap.net/) - libcoap implements a lightweight application-protocol for devices that are constrained their resources such as computing power, RF range, memory, bandwith, or network packet sizes
- [microcoap](https://github.com/1248/microcoap) -  A small CoAP implementation for microcontrollers
- [libnyoci](https://github.com/darconeous/libnyoci) -  A flexible CoAP stack for embedded devices and computers. RFC7252 compatible.

### CANopen

#### Open Source

- [CanFestival](http://www.canfestival.org/) - CanFestival focuses on providing an ANSI-C platform independent CANopen® stack that can be built as master or slave nodes on PCs, Real-time IPCs, and Microcontrollers.
- [CANopenNode](https://github.com/CANopenNode/CANopenNode) - CANopenNode is written in ANSI C in object-oriented way. It runs on different microcontrollers, as standalone application or with RTOS.
- [Lely CANopen Library](https://gitlab.com/lely_industries/co) - A CANopen implementation for both masters and slaves written in C, but with a C++ interface.

#### Proprietary

- [Ixxat](https://www.ixxat.com/products/products-industrial/protocol-software-and-apis/protocol-software/canopen-protocol-software)
- [port](http://www.port.de/en/products/canopen.html)
- [ESA's microCANopen Plus](http://www.canopenstore.com/pip/microcanopen-plus.html)
- [emtas](https://www.emtas.de/en/produkte/canopen-master-stack)
- [MicroControl](http://www.microcontrol.net/en/products/protocol-stacks/canopen/)

### Serialization

- [nanopb](https://koti.kapsi.fi/jpa/nanopb/) - Nanopb is a plain-C implementation of Google's Protocol Buffers data format. It is targeted at 32 bit microcontrollers, but is also fit for other embedded systems with tight (2-10 kB ROM, <1 kB RAM) memory constraints.
- [mpack](https://github.com/ludocode/mpack) - A C encoder/decoder for [MessagePack](http://msgpack.com) messages suitable for resource constriants embedded systems. Supports disabling dynamic memory allocation and overriding malloc, free, and realloc.
- [tinycbor](https://github.com/01org/tinycbor) - Intel's implementation of [CBOR](http://cbor.io/) designed for their IOT-based applications and processors
- [bitproto](https://github.com/hit9/bitproto) -  A fast, lightweight and easy-to-use bit level data interchange format for serializing data structure. Its syntax is similar to protobuf, but very suitable for the embedded systems.

### RTOS
#### Free or Open Source

- [TinyOS](https://github.com/tinyos/tinyos-main) - A operating system designed for low-power wireless devices, such as those used in sensor networks, ubiquitous computing, personal area networks, smart buildings, and smart meters.
- [ContikiOS](https://github.com/contiki-os/contiki) - A free Operating System with focus to provide standardized low-power wireless communication for a wide range of hardware platforms.
- [FreeRTOS](http://www.freertos.org/) - A free use Real Time Operating system which is widely used and supports a large number of platforms.
- [RIOT](https://github.com/RIOT-OS/)  - A free OS for IoT devices providing foundational trust services. The trust services include device identity, sealing, attestation, and data integrity. The term “Robust” is used because the minimal trusted computing base is tiny, and because RIoT capabilities can remotely re-establish trust in devices that have been compromised by malware.
- [RTEMS](https://www.rtems.org/) - Real-Time Executive for Multiprocessor Systems or RTEMS is an open source Real Time Operating System (RTOS) that supports open standard application programming interfaces (API) such as POSIX. It is used in space flight, medical, networking and many more embedded devices using processor architectures including ARM, PowerPC, Intel, Blackfin, MIPS, Microblaze and more.

#### Commercial

- [SafeRTOS](https://www.highintegritysystems.com/safertos/) - Certified version of FreeRTOS by TUEV SUED against IEC 61508 (basic functional safety standard) up to SIL3 (the highest safety integrity level for a single software component), ISO 26262 ASIL D (automotive standard) and EN62304 (medical device standard).
- [INTEGRITY/INTEGRITY-178](http://www.ghs.com/products/rtos/integrity.html#performance) - Two commercial RTOS variants targeting to power embedded systems with total reliability, absolute security, and maximum real-time performance. The variant INTEGRYTY-178 has a lot of safety and security certifications.
- [PikeOS](https://www.sysgo.com/products/pikeos-hypervisor/) - A commercial micro-kernel based operating system with a small footprint and certified for DO-178 (avionics), IEC-61508 (industrial), ISO-26262 (automotive).
- [Rocket](http://www.windriver.com/products/operating-systems/rocket/) - A free embedded operating system specifically designed to quickly and easily build small, intelligent devices in Wind Rivers cloud-based development environment, Wind River Helix™ App Cloud.
- [Nucleus RTOS](https://www.mentor.com/embedded-software/nucleus/) - Commercial, highly scalable micro-kernel based real-time operating system designed for scalability and reliability.
- [uC/os](https://www.micrium.com/rtos/kernels/) - µC/OS-II and µC/OS-III are preemptive, highly portable, and scalable real-time kernels. You can test them out for free, but you must pay to put them into a product.
- [TI-RTOS](www.ti.com/tool/ti-rtos) - A real-time operating system for TI microcontrollers, It Includes TCP/IP and USB stacks, a FAT file system, and device drivers, Most of the TI-RTOS components are released under the BSD License.

### Testing

- [CppUTest](https://cpputest.github.io/) - unit testing and mocking framework for C/C++ with a focus on working for embedded systems!
- [ceedling, unity and cmock](http://www.throwtheswitch.org/) - Unit testing, mocking and build framework written in C with ruby for generating and building.
- [doctest](https://github.com/onqtam/doctest) - A lightweight and feature-rich C++98/C++11 single-header testing framework for unit tests and TDD.
- [Mockitopp](https://github.com/tpounds/mockitopp) - A C++ mocking framework inspired by the ideas developed for Mockito written by Szczepan Faber, et al. The purpose is to provide similar construction semantics for creating mock objects leading to smaller, more readable test cases. It is designed to be a lightweight framework allowing you to mock dependencies for a system under test using a simple descriptive domain specific language. The goal is to help create simpler, less brittle test cases; ultimately, leading to less maintenance overhead in the future.
- [Trompeloeil](https://github.com/rollbear/trompeloeil) - A thread safe header only mocking framework for C++14 using the Boost Software License 1.0
- [Catch](https://github.com/catchorg/Catch2) - A modern, C++-native, header-only, test framework for unit-tests, TDD and BDD - using C++11, C++14, C++17 and later (or C++03 on the Catch1.x branch)

### Frameworks

- [Arduino](https://www.arduino.cc/)
- [AREG SDK](https://github.com/aregtech/areg-sdk) - An interface-centric real-time asynchronous communication engine for embedded and high-end applications to enable distributed- and [mist-computing](https://csrc.nist.gov/publications/detail/sp/500-325/final), where connected Things interact and provide services, as if they act like thin distributed servers.
- [ARM mbed](https://www.mbed.com/en/) - The ARM mbed IoT Device Platform provides the operating system, cloud services, tools and developer ecosystem to make the creation and deployment of commercial, standards-based IoT solutions possible at scale.

### Alternative Languages (Not C/C++)

#### D

- [minilibd](https://bitbucket.org/timosi/minlibd) - "This collection has libraries and tools to compile D language programs for embedded or "bare metal" systems with the
gdc compiler. The main focus is STM32 controllers but the library and build tools are easy to port to any processor."
- [DConf 2014 Talk "Tiny, Ubiquitous Machines Powered by D"](https://archive.org/details/dconf2014-day02-talk07) - Presentation about D in tiny embedded systems.

#### Rust
- [Zinc](https://zinc.rs/) - Bare-metal ARM stack for rust. Aimed at replacing CMSIS or mbed (currently defunct)
- [rust-embedded](https://github.com/rust-embedded/rfcs) - RFCs proposed by the Rust community for better embedded systems support.
- [embed.rs](http://embed.rs/) - Articles about doing embedded on rust

#### Elixir
- [Nerves](http://nerves-project.org/) - Uses buildroot to deploy Elixir programs running on the Erlang VM to embedded linux boards

#### Ada and Spark

- [AdaCore](https://github.com/AdaCore) - Open source maintainer of Ada with a focus on embedded use.

#### Javascript

- [Tessel](https://tessel.io/) - A openWRT based embedded system which can run Javascript.
- [JerryScript](https://github.com/Samsung/jerryscript) - A JavaScript engine intended to run on a very constrained devices such as microcontrollers. Designed for the Internet of Things.

#### Nim

- [Nim](https://nim-lang.org/) - A statically-typed programming language inspired by Python, Ada and Modula that compiles to C, C++, and Javascript.

#### Zig

- [Zig](https://ziglang.org/)

#### Clojure

- [Ferrett](https://ferret-lang.org/): Ferret is a free software Clojure implementation for real time embedded control systems.
  Generated code is self contained ISO C++11, it is not tied to any one compiler, generated code should be portable between any Operating System and/or Microcontroller that supports a C++11 compliant compiler. It has been verified to run on architectures ranging from embedded systems with as little as 2KB of RAM to general purpose computers running Linux/Mac OS X/Windows.

#### Golang

- [GERT](https://github.com/ycoroneos/G.E.R.T): GERT is a modified version of Go that runs bare-metal on armv7a SOCs. The minimal set of OS primitives that Go relies on have been re-implemented entirely in Go and Plan 9 assembly inside the modified runtime. The goal of this project is to bring the benefits of a high-level, type-safe, and garbage-collected language to bare-metal embedded environments.

#### MicroPython
- [MicroPython](https://micropython.org/) is a lean and efficient implementation of the Python 3 programming language that includes a small subset of the Python standard library and is optimised to run on microcontrollers and in constrained environments.

### STL

- [ESTL](https://github.com/esrlabs/estl-teaser) - C++ STL-like library for embedded developers with C++ 98 features only to maximize target platform compatibility.
- [ETL](https://github.com/etlcpp/etl) - Embedded Template Library which offers compile time defined container sizes, full C++ 03 and partial C++ 11 compatibility, deterministic behaviour, additional components for the embedded domain, etc.
- [uSTL](https://github.com/msharov/ustl) - Partial, code size implementation of the STL.
- [EASTL](https://github.com/electronicarts/EASTL) - Electronic Arts STL - aimed for console devices. Good descripton avaliable [HERE](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2007/n2271.html)

## Resources

### Other Lists

- [Single File Libs](https://github.com/nothings/single_file_libs) - Single File libraries for C++ and C. Some might be useful for embedded systems use.

### Podcasts

- [Embedded](http://embedded.fm/) - Elicia White and Christopher White interview makes, hackers and engineers who work on embedded systems
- [The Amp Hour](http://www.theamphour.com/)
- [Sparkgap](http://thesparkgap.net/)
- [Two's Complement Podcast](https://www.twoscomplement.org/) - Discussions between Matt Godbolt and Ben Rady, revolving around testing, best practices, etc in C and C++ development.

### Blogs

- [Embedded Artistry](https://embeddedartistry.com/) -
- [Interrupt](https://interrupt.memfault.com/blog/) - Great in-depth blog posts from MemFault. Mostly around ARM Cortex-M series processors.

### Newsletters

- [Embedsys Weekly](https://embedsysweekly.com/) - A weekly selection of embedded software and hardware articles.

### Videos

- [EEVBlog](https://www.eevblog.com/) - More on the electronics side, but David L. Jones tears apart embedded systems and electronic devices.
- [The Signal Path](https://thesignalpath.com/blogs/) - Electronics equipment teardowns

### Books

- Anderson, Ross J.: [Security Engineering: A Guide to Building Dependable Distributed Systems](http://eu.wiley.com/WileyCDA/WileyTitle/productCd-0470068523.html), John Wiley & Sons, 2nd, 2008 (ISBN-10: 0471389226, ISBN-13: 978-0471389224)
- Domeika, Max: [Software Development for Embedded Multi-core Systems: A Practical Guide Using Embedded Intel Architecture](https://www.elsevier.com/books/software-development-for-embedded-multi-core-systems/domeika/978-0-7506-8539-9), Newnes, 1st, 2008 (ISBN-10: 0750685395, ISBN-13: 978-0750685399)
- González, Alex: [Embedded Linux Projects Using Yocto Project Cookbook](https://www.packtpub.com/virtualization-and-cloud/embedded-linux-projects-using-yocto-project-cookbook), Packt Publishing Limited, 1st edition, 2015 (ISBN-10: 1784395188, ISBN-13: 9781784395186)
- Hagar, Jon Duncan: [Software Test Attacks to Break Mobile and Embedded Devices](https://www.crcpress.com/Software-Test-Attacks-to-Break-Mobile-and-Embedded-Devices/Hagar/p/book/9781466575301), Chapman & Hall/Crc, 1st, 2013 (ISBN-10: 1466575301, ISBN-13: 978-1466575301)
- Kopetz, Hermann: [Real-Time Systems: Design Principles for Distributed Embedded Applications (Real-Time Systems Series)](http://www.springer.com/de/book/9781441982360), Springer, 2nd, 2011 (ISBN-10: 1441982361, ISBN-13: 978-1441982360)
- Leveson, Nancy G.: [Engineering a Safer World: Systems Thinking Applied to Safety (Engineering Systems)](https://mitpress.mit.edu/books/engineering-safer-world), The MIT Press, 1st, 2012 (ISBN-10: 0262016621, ISBN-13:  978-0262016629)
- Medoff, Michael and Faller, Rainer: [Functional Safety: An IEC 61508 SIL 3 Compliant Development Process](https://www.amazon.com/Functional-Safety-Compliant-Development-Process/dp/193497708X/ref=sr_1_1?s=books&ie=UTF8&qid=1487104979&sr=1-1&keywords=An+IEC+61508+SIL+3+Compliant+Development+Process), exida.com LLC, 3rd, 2014 (ISBN-10: 193497708X, ISBN-13: 978-1934977088)
- Pathan, Al-Sakib Khan: [Securing Cyber-Physical Systems](https://www.crcpress.com/Securing-Cyber-Physical-Systems/Pathan/p/book/9781498700986), Crc Press Inc, 1st, 2015 (ISBN-10: 1498700985, ISBN-13: 978-1498700986)
- Rausand, Marvin: [Reliability of Safety-Critical Systems: Theory and Applications](http://eu.wiley.com/WileyCDA/WileyTitle/productCd-1118112725.html), Wiley, 1st, 2014 (ISBN-10: 1118112725, ISBN-13: 978-1118112724)
- Langr, Jeff: [Modern C++ Programming with Test-Driven Development - Code Better, Sleep Better](https://pragprog.com/book/lotdd/modern-c-programming-with-test-driven-development), OReilly, 1st edition, 2013 (ISBN-10: 1937785483, ISBN-13: 978-1937785482)
- Simmonds, Chris: [Mastering Embedded Linux Programming](https://www.packtpub.com/networking-and-servers/mastering-embedded-linux-programming), Packt Publishing Limited, 1st edition, 2015 (ISBN-10: 1784392537, ISBN-13: 9781784392536)
- [Making Embedded Systems by Elicia White](https://www.amazon.com/Making-Embedded-Systems-Patterns-Software/dp/1449302149) - Covers the basics of embedded systems architecture, design and patterns.
- [Test Driven Developmet for Embedded C by James Grenning](https://www.amazon.com/Driven-Development-Embedded-Pragmatic-Programmers/dp/193435662X/ref=asap_bc?ie=UTF8) - How to approach test driven development for embedded devices written in C.
- [uC/OS-III, The Real-Time Kernel by Jean J Labrosse](https://www.amazon.com/dp/0982337531/ref=pd_lpo_sbs_dp_ss_3?pf_rd_p=1944687682&pf_rd_s=lpo-top-stripe-1&pf_rd_t=201&pf_rd_i=1578201039&pf_rd_m=ATVPDKIKX0DER&pf_rd_r=SVE997FF9MNQ1VYEJCM1) - A book about the Micrium's uC/os III. It is a great resource on how RTOSes for embedded systems should work.
- [An Embedded Software Primer by David E. Simon](https://www.amazon.com/Embedded-Software-Primer-David-Simon/dp/020161569X) - An introduction to embedded systems, with a good explanation to Real-time operating systems(RTOS).

### Standards

- [Embedded C Coding Standards](http://www.barrgroup.com/Embedded-Systems/Books/Embedded-C-Coding-Standard) - Coding standards for embedded C from the Barr Group.
- [SEI CERT C Coding Standard](https://wiki.sei.cmu.edu/confluence/display/c/SEI+CERT+C+Coding+Standard) - The SEI CERT C Coding Standard is a software coding standard for the C programming language to improve the safety, reliability, and security of software systems.

### Tools

- [PlatformIO](http://platformio.org/) - PlatformIO is an open source ecosystem for IoT development
Cross-platform build system. Continuous and IDE integration. Arduino and ARM mbed compatible
- [Energia](http://energia.nu) - Energia is an open-source electronics prototyping platform, it brings the Wiring and Arduino framework to the Texas Instruments MSP430 based LaunchPad, it includes an IDE that is based on Processing.
- [XOD](https://xod.io) - An open source visual programming platform for Arduino-compatible boards.

### Embedded Linux

- [yocto](https://www.yoctoproject.org/) - Yocto is a tool for creating custom embedded linux systems
- [Buildroot](https://buildroot.org/) - Buildroot is a simple, efficient and easy-to-use tool to generate embedded Linux systems through cross-compilation.
- [Mender](https://github.com/mendersoftware/mender) - Open source over-the-air (OTA) software updater for embedded Linux devices.
- [SWUpdate](https://github.com/sbabic/swupdate) - Linux Update agent with the goal to provide an efficient and safe way to update (local, remote, multiple update strategies) an embedded system.

### Courses

- [C++ programming in Qt FrameWork Part I (udemy)](https://www.udemy.com/c-programming-creating-applications-with-qt-framework/) - not free
- [C++ programming in Qt Framework: Part II (udemy)](https://www.udemy.com/c-programming-in-qt-framework-part-ii) - not free
- [Computer Systems Design for Energy Efficiency (edx)](https://www.edx.org/course/computer-systems-design-energy-chalmersx-chm007x)
- [Cybersecurity Fundamentals - Construction of Secure Systems (coursera)](https://www.coursera.org/specializations/cyber-security) Landing page for 5 courses about security with relation to embedded systems.
- [Development of Real-Time Systems (coursera)](https://www.coursera.org/learn/real-time-systems)
- [Embedded Systems - Shape The World (edx)](https://www.edx.org/course/embedded-systems-shape-world-utaustinx-ut-6-03x)
- [FPGA Turbo Series - Communication Protocols](https://www.udemy.com/fpga-turbo-series-communication-protocols/)
- [FPGA Turbo Series - Implementing a UART](https://www.udemy.com/fpga-turbo-series-uart/)
- [Fun & Easy Embedded Microcontroller Communication Protocols (Udemy)](https://www.udemy.com/fun-easy-embedded-microcontroller-communication-protocols/) - Content: I2C/TWI, SPI, UART, MODBUS RTU, CAN, USB, ETHERNET, PCIE
- [Introduction to Qt: A C++ Cross Platform Application Framework (pluralsight)](https://www.pluralsight.com/courses/introduction-qt-cplusplus-framework) - not free
- [Integrating Qt Quick with C++ (pluralsight)](https://www.pluralsight.com/courses/integrating-qt-quick-cpp) - not free
- [Learn FreeRTOS from scratch](https://www.udemy.com/freertos-getting-started/) - not free - Learn about FreeRTOS basics. Practise it's APIs with different examples.
- [Linux OS in Embedded Systems & Linux Kernel Internals(1/2) (Udemy)](https://www.udemy.com/becoming-linux-expert-series-install-linux-operating-system/) - not free
- [Linux OS in Embedded Systems & Linux Kernel Internals(2/2) (Udemy)](https://www.udemy.com/c-complete-reference/) - not free
- [ARM Cortex-M Bare-Metal Embedded-C Programming (Udemy)](https://www.udemy.com/cortex-m-internals-master-pointers-structures-memory-etc/)
- [ARM Cortex-M Assembly Programming (Udemy)](https://www.udemy.com/arm-cortex-m-assembly-programming/)
- [Introduction to Embedded Systems using 8051 Microcontroller (Udemy)](https://www.udemy.com/introduction-to-embedded-systems-using-8051-microcontroller/)
- [Mastering Microcontroller with Peripheral Driver Development (Udemy)](https://www.udemy.com/mastering-microcontroller-with-peripheral-driver-development/)
- [Embedded Systems Programming on ARM Cortex-M3/M4 Processor (Udemy)](https://www.udemy.com/embedded-system-programming-on-arm-cortex-m3m4/)
- [Foundation course on Embedded Linux (Udemy)](https://www.udemy.com/foundation-course-on-embedded-linux/)
- [Hands-on Embedded Systems, ARM Cortex Tutorials - ADCs (Udemy)](https://www.udemy.com/armcortex-adc/)
- [edX Embedded Systems Course by University of Texas Austin](https://www.edx.org/course/embedded-systems-shape-world-utaustinx-ut-6-03x)
- [System Validation (1): Automata and behavioural equivalences (coursera)](https://www.coursera.org/learn/automata-system-validation)
- [System Validation (2): Model process behaviour (coursera)](https://www.coursera.org/learn/system-validation-behavior)
- [UNC Charlotte Embedded Systems Course](https://www.youtube.com/playlist?list=PLE4462C1C306E2EB2)
- [QT C++ GUI Tutorial For Beginners (udemy)](https://www.udemy.com/qt-c-gui-tutorial-for-beginners/) - not free
- [How To Implement Your First VHDL Design on FPGA (udemy)](https://www.udemy.com/how-to-implement-your-first-vhdl-design-on-fpga/)
- [Learn VHDL and FPGA Development (udemy)](https://www.udemy.com/vhdl-and-fpga-development-for-beginners-and-intermediates/)
- [FPGA Design Learning VHDL (udemy)](https://www.udemy.com/fpga-design-learning-vhdl/)
- [Learn VHDL Design for use in FPGA and ASIC Digital Systems (udemy)](https://www.udemy.com/vhdl-design-and-modeling-of-digital-systems/)
- [Learn VHDL, ISE and FPGA by Designing a basic Home Alarm (udemy)](https://www.udemy.com/getting-started-with-fpga-ise-and-vhdl/)
- [The Embedded Pre-Interview! (udemy)](https://www.udemy.com/the-embedded-pre-interview/) - not free - Evaluate your Embedded Systems knowledge, in just 100 minutes, for any entry level job

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Chris Woodall](http://cwoodall.com) has waived all copyright and related or neighboring rights to this work.
