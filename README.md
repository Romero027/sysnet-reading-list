# System/Networking Paper Reading List
This repository contains a list of papers on various topics (that I am currently working on) in the system and networking area.


## Index 

* [Middleboxs and NFV](#middleboxes-and-nfv)
* [eBPF and XDP](#ebpf-and-xdp)
* [Transport Protocol](#transport-protocol)
* [Microservice and Service Mesh](#microservice-and-service-mesh)
* [Network Stack](#network-stack)
* [Internet Architecture](#internet-architecture)
* [Container Networking](#container-networking)

***

### Middleboxs and NFV
- [**The Click Modular Router**](https://dl.acm.org/doi/10.1145/354871.354874), _TOCS '00_
- [**Middleboxes No Longer Considered Harmful**](http://nms.lcs.mit.edu/papers/doa-osdi04.pdf), _OSDI '04_
- [**Design and Implementation of a Consolidated Middlebox Architecture**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/sekar), _NSDI '12_
- [**mOS: A Reusable Networking Stack for Flow Monitoring Middleboxes**](https://www.usenix.org/conference/nsdi17/technical-sessions/presentation/jamshed), _NSDI'17_
- [**ClickNF: a Modular Stack for Custom Network Functions**](https://www.usenix.org/conference/atc18/presentation/gallo), _ATC '18_
- [**Programming Network Stack for Middleboxes with Rubik**](https://www.usenix.org/conference/nsdi21/presentation/li), _NSDI '21_

### eBPF and XDP
- [**The eXpress data path: fast programmable packet processing in the operating system kernel**](https://dl.acm.org/doi/10.1145/3281411.3281443), _CoNEXT '18_
- [**hXDP: Efficient Software Packet Processing on FPGA NICs**](https://www.usenix.org/conference/osdi20/presentation/brunella), _OSDI '20_
- [**BPF for storage: an exokernel-inspired approach**](https://dl.acm.org/doi/10.1145/3458336.3465290), _HotOS '21_
- [**BMC: Accelerating Memcached using Safe In-kernel Caching and Pre-stack Processing**](https://www.usenix.org/conference/nsdi21/presentation/ghigoff), _NSDI '21_
- [**Synthesizing Safe and Efficient Kernel Extensions for Packet Processing**](https://dl.acm.org/doi/pdf/10.1145/3452296.3472929), _SIGCOMM '21_
- [**Syrup: User-Defined Scheduling Across the Stack**](https://dl.acm.org/doi/pdf/10.1145/3477132.3483548), _SOSP '21_

### Transport Protocol
- [**Homa: A Receiver-Driven Low-Latency Transport Protocol Using Network Priorities**](https://dl.acm.org/doi/10.1145/3230543.3230564), _SIGCOMMM '18_
- [**R2P2: Making RPCs first-class datacenter citizens**](https://www.usenix.org/conference/atc19/presentation/kogias-r2p2), _ATC '19_
- [**TCP is Harmful to In-Network Computing: Designing a Message Transport Protocol (MTP)**](https://dl.acm.org/doi/10.1145/3484266.3487382), _HotNets '21_


### Microservice and Service Mesh
- [**Service Fabric: A Distributed Platform for Building Microservices in the Cloud**](https://dl.acm.org/doi/10.1145/3190508.3190546), _EuroSys '18_
- [**An Open-Source Benchmark Suite for Microservices and Their Hardware-Software Implications for Cloud & Edge Systems**](https://dl.acm.org/doi/10.1145/3297858.3304013), _ASPLOS '19_
- [**E3: Energy-Efficient Microservices on SmartNIC-Accelerated Servers**](https://www.usenix.org/conference/atc19/presentation/liu-ming), _ATC '19_
- [**Leveraging Service Meshes as a New Network Layer**](https://dl.acm.org/doi/abs/10.1145/3484266.3487379), _HotNets '21_

### Network Stack
- [**Network stack specialization for performance**](https://dl.acm.org/doi/10.1145/2619239.2626311), _SIGCOMM '14_
- [**RSS++: load and state-aware receive side scaling**](https://dl.acm.org/doi/10.1145/3359989.3365412), _CoNEXT '19_
- [**Understanding Host Network Stack Overheads**](https://dl.acm.org/doi/abs/10.1145/3452296.3472888), _SIGCOMM '20_

### Internet Architecture
- [**Architectural considerations for a new generation of protocols**](https://dl.acm.org/doi/10.1145/99517.99553), _SIGCOMM CCR '90_
- [**Networking named content**](https://dl.acm.org/doi/10.1145/1658939.1658941), _CoNEXT '12_
- [**XIA: Efficient Support for Evolvable Internetworking**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/han_dongsu_xia), _NSDI '12_
- [**Serval: An End-Host Stack for Service-Centric Networking**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/nordstrom), _NSDI '12_

### Container Networking
- [**Slipstream: Automatic Interprocess Communication Optimization**](https://www.usenix.org/conference/atc15/technical-session/presentation/dietz), _ATC '15_
- [**Iron: Isolating Network-based CPU in Container Environments**](https://www.usenix.org/conference/nsdi18/presentation/khalid), _NSDI '18_
- [**FreeFlow: Software-based Virtual RDMA Networking for Containerized Clouds**](https://www.usenix.org/conference/nsdi19/presentation/kim), _NSDI '19_
- [**Slim: OS Kernel Support for a Low-Overhead Container Overlay Network**](https://www.usenix.org/conference/nsdi19/presentation/zhuo), _NSDI '19_
- [**Particle: Ephemeral Endpoints for Serverless Networking**](https://dl.acm.org/doi/10.1145/3419111.3421275), _SoCC '20_
- [**Parallelizing packet processing in container overlay networks**](https://dl.acm.org/doi/10.1145/3447786.3456241), _EuroSys '21_
