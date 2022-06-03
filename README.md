# System/Networking Paper Reading List

## Index 

* [**Middleboxs and NFV**](#middleboxes-and-nfv)
* [**eBPF and XDP**](#ebpf-and-xdp)
* [**Transport Protocol**](#transport-protocol)
* [**Microservice and Service Mesh**](#microservice-and-service-mesh)
* [**Network Stack**](#network-stack)
* [**Internet Architecture**](#internet-architecture)
* [**Container Networking**](#container)

## Reading List

### Middleboxs and NFV
- [**The Click Modular Router**](https://dl.acm.org/doi/10.1145/354871.354874), _TOCS '00_
- [**Middleboxes No Longer Considered Harmful**](http://nms.lcs.mit.edu/papers/doa-osdi04.pdf), _OSDI '04_
- [**Making Middleboxes Someone Else’s Problem: Network Processing as a Cloud Service**](https://dl.acm.org/doi/10.1145/2342356.2342359), _SIGCOMM '12_
- [**Design and Implementation of a Consolidated Middlebox Architecture**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/sekar), _NSDI '12_
- [**ClickOS and the Art of Network Function Virtualization**](https://www.usenix.org/conference/nsdi14/technical-sessions/presentation/martins), _NSDI'14_
- [**NetBricks: Taking the V out of NFV**](https://www.usenix.org/conference/osdi16/technical-sessions/presentation/panda), _OSDI '16_
- [**Paving the Way for NFV: Simplifying Middlebox Modifications Using StateAlyzr**](https://www.usenix.org/conference/nsdi16/technical-sessions/presentation/khalid), _NSDI'16_
- [**mOS: A Reusable Networking Stack for Flow Monitoring Middleboxes**](https://www.usenix.org/conference/nsdi17/technical-sessions/presentation/jamshed), _NSDI'17_
- [**Metron: NFV Service Chains at the True Speed of the Underlying Hardware**](https://www.usenix.org/conference/nsdi18/presentation/katsikas), _NSDI'18_
- [**Microboxes: High Performance NFV with Customizable, Asynchronous TCP Stacks and Dynamic Subscriptions**](https://dl.acm.org/doi/pdf/10.1145/3230543.3230563), _SIGCOMM '18_
- [**ClickNF: a Modular Stack for Custom Network Functions**](https://www.usenix.org/conference/atc18/presentation/gallo), _ATC '18_
- [**Performance Contracts for Software Network Functions**](https://www.usenix.org/conference/nsdi19/presentation/iyer), _NSDI '19_
- [**Gallium: Automated Software Middlebox Offloading to Programmable Switches**](https://dl.acm.org/doi/abs/10.1145/3387514.3405869), _SIGCOMM '20_
- [**Programming Network Stack for Middleboxes with Rubik**](https://www.usenix.org/conference/nsdi21/presentation/li), _NSDI '21_

### eBPF and XDP
- [**The eXpress data path: fast programmable packet processing in the operating system kernel**](https://dl.acm.org/doi/10.1145/3281411.3281443), _CoNEXT '18_
- [**hXDP: Efficient Software Packet Processing on FPGA NICs**](https://www.usenix.org/conference/osdi20/presentation/brunella), _OSDI '20_
- [**Specification and verification in the field: Applying formal methods to BPF just-in-time compilers in the Linux kernel**](https://www.usenix.org/conference/osdi20/presentation/nelson), _OSDI '20_
- [**BPF for storage: an exokernel-inspired approach**](https://dl.acm.org/doi/10.1145/3458336.3465290), _HotOS '21_
- [**BMC: Accelerating Memcached using Safe In-kernel Caching and Pre-stack Processing**](https://www.usenix.org/conference/nsdi21/presentation/ghigoff), _NSDI '21_
- [**Synthesizing Safe and Efficient Kernel Extensions for Packet Processing**](https://dl.acm.org/doi/pdf/10.1145/3452296.3472929), _SIGCOMM '21_
- [**Syrup: User-Defined Scheduling Across the Stack**](https://dl.acm.org/doi/pdf/10.1145/3477132.3483548), _SOSP '21_

### Transport Protocol
- [**The QUIC Transport Protocol: Design and Internet-Scale Deployment**](https://dl.acm.org/doi/10.1145/3484266.3487382), _SIGCOMM '17_
- [**Homa: A Receiver-Driven Low-Latency Transport Protocol Using Network Priorities**](https://dl.acm.org/doi/10.1145/3230543.3230564), _SIGCOMMM '18_
- [**R2P2: Making RPCs first-class datacenter citizens**](https://www.usenix.org/conference/atc19/presentation/kogias-r2p2), _ATC '19_
- [**TCP is Harmful to In-Network Computing: Designing a Message Transport Protocol (MTP)**](https://dl.acm.org/doi/10.1145/3484266.3487382), _HotNets '21_


### Microservice and Service Mesh
- [**Service Fabric: A Distributed Platform for Building Microservices in the Cloud**](https://dl.acm.org/doi/10.1145/3190508.3190546), _EuroSys '18_
- [**Overload Control for Scaling WeChat Microservices**](https://dl.acm.org/doi/10.1145/3267809.3267823), _SoCC '18_
- [**µTune: Auto-Tuned Threading for OLDI Microservices**](https://www.usenix.org/conference/osdi18/presentation/sriraman), _OSDI '18_
- [**An Open-Source Benchmark Suite for Microservices and Their Hardware-Software Implications for Cloud & Edge Systems**](https://dl.acm.org/doi/10.1145/3297858.3304013), _ASPLOS '19_
- [**Seer: Leveraging Big Data to Navigate the Complexity of Performance Debugging in Cloud Microservices**](https://dl.acm.org/doi/10.1145/3297858.3304004), _ASPLOS '19_
- [**PARTIES: QoS-Aware Resource Partitioning for Multiple Interactive Services**](https://dl.acm.org/doi/pdf/10.1145/3297858.3304005), _ASPLOS '19_
- [**E3: Energy-Efficient Microservices on SmartNIC-Accelerated Servers**](https://www.usenix.org/conference/atc19/presentation/liu-ming), _ATC '19_
- [**Autopilot: workload autoscaling at Google**](https://dl.acm.org/doi/pdf/10.1145/3342195.3387524), _EuroSys '20_
- [**FIRM: An Intelligent Fine-grained Resource Management Framework for SLO-Oriented Microservices**](https://www.usenix.org/conference/osdi20/presentation/qiu), _OSDI '20_
- [**Nightcore: Efficient and Scalable Serverless Computing for Latency-Sensitive, Interactive Microservices**](https://dl.acm.org/doi/pdf/10.1145/3445814.3446701), _ASPLOS '21_
- [**Sage: Practical and Scalable ML-Driven Performance Debugging in Microservices**](https://dl.acm.org/doi/pdf/10.1145/3445814.3446700), _ASPLOS '21_
- [**Sinan: ML-Based and QoS-Aware Resource Management for Cloud Microservices**](https://dl.acm.org/doi/pdf/10.1145/3445814.3446693), _ASPLOS '21_
- [**Characterizing Microservice Dependency and Performance: Alibaba Trace Analysis**](https://dl.acm.org/doi/pdf/10.1145/3472883.3487003), _SoCC '21_
- [**Leveraging Service Meshes as a New Network Layer**](https://dl.acm.org/doi/abs/10.1145/3484266.3487379), _HotNets '21_
- [**DeepRest: Deep Resource Estimation for Interactive Microservices**](https://dl.acm.org/doi/pdf/10.1145/3492321.3519564), _EuroSys '22_

### Network Stack
- [**mTCP: a Highly Scalable User-level TCP Stack for Multicore Systems**](https://www.usenix.org/conference/nsdi14/technical-sessions/presentation/jeong), _NSDI '14_
- [**Network stack specialization for performance**](https://dl.acm.org/doi/10.1145/2619239.2626311), _SIGCOMM '14_
- [**IX: A Protected Dataplane Operating System for High Throughput and Low Latency**](https://www.usenix.org/conference/osdi14/technical-sessions/presentation/belay), _OSDI '14
- [**Arrakis: The Operating System is the Control Plane**](https://www.usenix.org/conference/osdi14/technical-sessions/presentation/peter), _OSDI '14_
- [**StackMap: Low-Latency Networking with the OS Stack and Dedicated NICs**](https://www.usenix.org/conference/atc16/technical-sessions/presentation/yasukata), _ATC '16_
- [**ModNet: A Modular Approach to Network Stack Extension**](https://www.usenix.org/conference/nsdi15/technical-sessions/presentation/pathak), NSDI '15_
- [**RSS++: load and state-aware receive side scaling**](https://dl.acm.org/doi/10.1145/3359989.3365412), _CoNEXT '19_
- [**TAS: TCP Acceleration as an OS Service**](https://dl.acm.org/doi/10.1145/3302424.3303985), _SIGCOMM '19_
- [**Snap: a Microkernel Approach to Host Networking**](https://dl.acm.org/doi/10.1145/3341301.3359657), SOSP '19_
- [**SocksDirect: Datacenter Sockets can be Fast and Compatible**](https://dl.acm.org/doi/10.1145/3341302.3342071), _SIGCOMM '19_
- [**Understanding Host Network Stack Overheads**](https://dl.acm.org/doi/abs/10.1145/3452296.3472888), _SIGCOMM '20_

### Internet Architecture
- [**Architectural considerations for a new generation of protocols**](https://dl.acm.org/doi/10.1145/99517.99553), _SIGCOMM CCR '90_
- [**A Data-Oriented (and Beyond) Network Architecture**](https://dl.acm.org/doi/pdf/10.1145/1282380.1282402), SIGCOMM '07_
- [**Networking named content**](https://dl.acm.org/doi/10.1145/1658939.1658941), _CoNEXT '12_
- [**XIA: Efficient Support for Evolvable Internetworking**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/han_dongsu_xia), _NSDI '12_
- [**Serval: An End-Host Stack for Service-Centric Networking**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/nordstrom), _NSDI '12_
- [**Enabling a Permanent Revolution in Internet Architecture**](https://dl.acm.org/doi/pdf/10.1145/3341302.3342075), _SIGCOMM '19_


### Container
- [**Slipstream: Automatic Interprocess Communication Optimization**](https://www.usenix.org/conference/atc15/technical-session/presentation/dietz), _ATC '15_
- [**Slacker: Fast Distribution with Lazy Docker Containers**](https://www.usenix.org/conference/fast16/technical-sessions/presentation/harter), _FAST '16_
- [**Improving Docker Registry Design Based on Production Workload Analysis**](https://www.usenix.org/conference/fast18/presentation/anwar), _FAST '18_
- [**Cntr: Lightweight OS Containers**](https://www.usenix.org/conference/atc18/presentation/thalheim), _ATC '18_
- [**Iron: Isolating Network-based CPU in Container Environments**](https://www.usenix.org/conference/nsdi18/presentation/khalid), _NSDI '18_
- [**FreeFlow: Software-based Virtual RDMA Networking for Containerized Clouds**](https://www.usenix.org/conference/nsdi19/presentation/kim), _NSDI '19_
- [**Slim: OS Kernel Support for a Low-Overhead Container Overlay Network**](https://www.usenix.org/conference/nsdi19/presentation/zhuo), _NSDI '19_
- [**Particle: Ephemeral Endpoints for Serverless Networking**](https://dl.acm.org/doi/10.1145/3419111.3421275), _SoCC '20_
- [**Parallelizing packet processing in container overlay networks**](https://dl.acm.org/doi/10.1145/3447786.3456241), _EuroSys '21_
- [**Starlight: Fast Container Provisioning on the Edge and over the WAN**](https://www.usenix.org/conference/nsdi22/presentation/chen-jun-lin), _NSDI '22_
