# System/Networking Paper Reading List

## Index 

* [**Middleboxs and NFV**](#middleboxs-and-nfv)
* [**Network Abstractions**](#network-abstraction--language)
* [**eBPF and XDP**](#ebpf-and-xdp)
* [**Transport Protocol**](#transport-protocol)
* [**Microservice and Service Mesh**](#microservice-and-service-mesh)
* [**Network Stack**](#network-stack-and-rpc-optimization)
* [**Workload Interference**](#workload-interference)
* [**Internet Architecture**](#internet-architecture)
* [**Container Networking**](#container)

## Reading List

### Middleboxs and NFV
- [**The Click Modular Router**](https://dl.acm.org/doi/10.1145/354871.354874), _TOCS '00_
- [**Middleboxes No Longer Considered Harmful**](http://nms.lcs.mit.edu/papers/doa-osdi04.pdf), _OSDI '04_
- [**Making Middleboxes Someone Else’s Problem: Network Processing as a Cloud Service**](https://dl.acm.org/doi/10.1145/2342356.2342359), _SIGCOMM '12_
- [**Design and Implementation of a Consolidated Middlebox Architecture**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/sekar), _NSDI '12_
  - Today's middleboxes are independent, specialized boxes. CoMb consolidates middleboxes to exploit multiplexing, module reuse, and spatial distribution
- [**Split/Merge: System Support for Elastic Execution in Virtual Middleboxes**](https://www.usenix.org/conference/nsdi13/technical-sessions/presentation/rajagopalan), _NSDI'14_
  - Autoscaling of stateful network functions 
- [**ClickOS and the Art of Network Function Virtualization**](https://www.usenix.org/conference/nsdi14/technical-sessions/presentation/martins), _NSDI'14_
- [**Enforcing Network-Wide Policies in the Presence of Dynamic Middlebox Actions using FlowTags**](https://www.usenix.org/conference/nsdi14/technical-sessions/presentation/fayazbakhsh), _NSDI'14_
- [**BlindBox: Deep Packet Inspection over Encrypted Traffic**](https://dl.acm.org/doi/10.1145/2829988.2787502), _SIGCOMM'15_
- [**Rollback-Recovery for Middleboxes**](https://dl.acm.org/doi/10.1145/2829988.2787501), _SIGCOMM'15_
- [**NetBricks: Taking the V out of NFV**](https://www.usenix.org/conference/osdi16/technical-sessions/presentation/panda), _OSDI '16_
- [**OpenBox: A Software-Defined Framework for Developing, Deploying, and Managing Network Functions**](https://dl.acm.org/doi/10.1145/2934872.2934875), _SIGCOMM'16_
- [**Paving the Way for NFV: Simplifying Middlebox Modifications Using StateAlyzr**](https://www.usenix.org/conference/nsdi16/technical-sessions/presentation/khalid), _NSDI'16_
- [**Stateless Network Functions: Breaking the Tight Coupling of State and Processing**](https://www.usenix.org/conference/nsdi17/technical-sessions/presentation/kablan), _NSDI'17_
- [**NFP: Enabling Network Function Parallelism in NFV**](https://dl.acm.org/doi/10.1145/3098822.3098826), _SIGCOMM'17_
- [**NFVnice: Dynamic Backpressure and Scheduling for NFV Service Chains**](https://dl.acm.org/doi/10.1145/3098822.3098828), _SIGCOMM'17_
- [**Metron: NFV Service Chains at the True Speed of the Underlying Hardware**](https://www.usenix.org/conference/nsdi18/presentation/katsikas), _NSDI'18_
- [**Elastic Scaling of Stateful Network Functions**](https://www.usenix.org/conference/nsdi18/presentation/woo), _NSDI'18_
- [**ResQ: Enabling SLOs in Network Function Virtualization**](https://www.usenix.org/conference/nsdi18/presentation/tootoonchian), _NSDI'18_
- [**Microboxes: High Performance NFV with Customizable, Asynchronous TCP Stacks and Dynamic Subscriptions**](https://dl.acm.org/doi/pdf/10.1145/3230543.3230563), _SIGCOMM '18_
- [**ClickNF: a Modular Stack for Custom Network Functions**](https://www.usenix.org/conference/atc18/presentation/gallo), _ATC '18_
- [**FlowBlaze: Stateful Packet Processing in Hardware**](https://www.usenix.org/conference/nsdi19/presentation/pontarelli), _NSDI '19_
- [**Performance Contracts for Software Network Functions**](https://www.usenix.org/conference/nsdi19/presentation/iyer), _NSDI '19_
- [**Correctness and Performance for Stateful Chained Network Functions**](https://www.usenix.org/conference/nsdi19/presentation/khalid), _NSDI '19_
- [**Verifying software network functions with no verification expertise**](https://dl.acm.org/doi/10.1145/3341301.3359647), _SOSP '19_
- [**Gallium: Automated Software Middlebox Offloading to Programmable Switches**](https://dl.acm.org/doi/abs/10.1145/3387514.3405869), _SIGCOMM '20_
- [**TEA: Enabling State-Intensive Network Functions on Programmable Switches**](https://dl.acm.org/doi/10.1145/3387514.3405855), _SIGCOMM '20_
- [**Contention-Aware Performance Prediction For Virtualized Network Functions**](https://dl.acm.org/doi/abs/10.1145/3387514.3405868), _SIGCOMM '20_ 
- [**SNF: serverless network functions**](https://dl.acm.org/doi/10.1145/3419111.3421295), _SoCC '20_ 
- [**Performance Interfaces for Network Functions**](https://www.usenix.org/conference/nsdi22/presentation/iyer), _NSDI '22_
- [**Quadrant: A Cloud-Deployable NF Virtualization Platform**](https://dl.acm.org/doi/pdf/10.1145/3542929.3563471), _SoCC '22_
- [**A High-Speed Stateful Packet Processing Approach for Tbps Programmable Switches**](https://www.usenix.org/conference/nsdi23/presentation/scazzariello), _NSDI '23_
- [**ExoPlane: An Operating System for On-Rack Switch Resource Augmentation**](https://www.usenix.org/conference/nsdi23/presentation/kim-daehyeok), _NSDI '23_
- [**LemonNFV: Consolidating Heterogeneous Network Functions at Line Speed**](https://www.usenix.org/conference/nsdi23/presentation/li-hao), _NSDI '23_
  - Consolidate unmodified NFs that are implemented in different platforms (e.g., Snort, Click, and NetBricks)
- [**Disaggregating Stateful Network Functions**](https://www.usenix.org/conference/nsdi23/presentation/bansal), _NSDI '23_
- [**Automatic Parallelization of Software Network Functions**](https://www.usenix.org/conference/nsdi24/presentation/pereira), _NSDI '24_

### Network Abstraction / Language
- [**Chimera: A Declarative Language for Streaming Network Traffic Analysis**](https://www.usenix.org/conference/usenixsecurity12/technical-sessions/presentation/borders), _Security '12_
- [**Abstractions for network update**](https://dl.acm.org/doi/10.1145/2342356.2342427), _SIGCOMM '12_
- [**Compiling Path Queries**](https://www.usenix.org/conference/nsdi16/technical-sessions/presentation/narayana), _NSDI '16_
- [**SNAP: Stateful Network-Wide Abstractions for Packet Processing**](https://dl.acm.org/doi/10.1145/2934872.2934892), _SIGCOMM '16_
- [**mOS: A Reusable Networking Stack for Flow Monitoring Middleboxes**](https://www.usenix.org/conference/nsdi17/technical-sessions/presentation/jamshed), _NSDI'17_
- [**Quantitative Network Monitoring with NetQRE**](https://dl.acm.org/doi/10.1145/3098822.3098830), _SIGCOMM '17_
- [**Language-Directed Hardware Design for Network Performance Monitoring**](https://dl.acm.org/doi/10.1145/3098822.3098829), _SIGCOMM '17_
- [**Sonata: query-driven streaming network telemetry**](https://dl.acm.org/doi/10.1145/3230543.3230555), _SIGCOMM '18_
- [**Lyra: A Cross-Platform Language and Compiler for Data Plane Programming on Heterogeneous ASICs**](https://dl.acm.org/doi/10.1145/3387514.3405879), _SIGCOMM '20_
- [**Lucid: a language for control in the data plane**](https://dl.acm.org/doi/10.1145/3452296.3472903), _SIGCOMM '21_
- [**Programming Network Stack for Middleboxes with Rubik**](https://www.usenix.org/conference/nsdi21/presentation/li), _NSDI '21_
  - Designed a language for programming middleboxes with an emphasis on supporting various transport protocols and flexible network stack hierarchy.
- [**SwiSh: Distributed Shared State Abstractions for Programmable Switches**](https://www.usenix.org/conference/nsdi22/presentation/zeno), _NSDI '22_
- [**NetRPC: Enabling In-Network Computation in Remote Procedure Calls**](https://www.usenix.org/conference/nsdi23/presentation/zhao-bohan), _NSDI '23_
- [**ClickINC: In-network Computing as a Service in Heterogeneous Programmable Data-center Networks**](https://dl.acm.org/doi/10.1145/3603269.3604835), _SIGCOMM '23_

### eBPF and XDP (See Also [awesome-ebpf](https://github.com/zoidbergwill/awesome-ebpf/tree/master))
- [**The eXpress data path: fast programmable packet processing in the operating system kernel**](https://dl.acm.org/doi/10.1145/3281411.3281443), _CoNEXT '18_
- [**hXDP: Efficient Software Packet Processing on FPGA NICs**](https://www.usenix.org/conference/osdi20/presentation/brunella), _OSDI '20_
- [**Specification and verification in the field: Applying formal methods to BPF just-in-time compilers in the Linux kernel**](https://www.usenix.org/conference/osdi20/presentation/nelson), _OSDI '20_
- [**BPF for storage: an exokernel-inspired approach**](https://dl.acm.org/doi/10.1145/3458336.3465290), _HotOS '21_
- [**BMC: Accelerating Memcached using Safe In-kernel Caching and Pre-stack Processing**](https://www.usenix.org/conference/nsdi21/presentation/ghigoff), _NSDI '21_
- [**Synthesizing Safe and Efficient Kernel Extensions for Packet Processing**](https://dl.acm.org/doi/pdf/10.1145/3452296.3472929), _SIGCOMM '21_
- [**ghOSt: Fast & Flexible User-Space Delegation of Linux Scheduling**](https://dl.acm.org/doi/10.1145/3477132.3483542), _SOSP '21_
- [**Syrup: User-Defined Scheduling Across the Stack**](https://dl.acm.org/doi/pdf/10.1145/3477132.3483548), _SOSP '21_
- [**LiteFlow: towards high-performance adaptive neural networks for kernel datapath**](https://dl.acm.org/doi/10.1145/3544216.3544229), _SIGCOMM '22_
- [**XRP: In-Kernel Storage Functions with eBPF**](https://www.usenix.org/conference/osdi22/presentation/zhong), _OSDI '22_
- [**Electrode: Accelerating Distributed Protocols with eBPF**](https://www.usenix.org/conference/nsdi23/presentation/zhou), _NSDI '23_
- [**Tigger: A Database Proxy That Bounces With User-Bypass**](https://www.vldb.org/pvldb/vol16/p3335-butrovich.pdf), _VLDB '23_
- [**Automatic Kernel Offload Using BPF**](https://dl.acm.org/doi/10.1145/3593856.3595888), _HotOS '23_
- [**EPF: Evil Packet Filter**](https://www.usenix.org/conference/atc23/presentation/jin), _ATC '23_
- [**DINT: Fast In-Kernel Distributed Transactions with eBPF**](https://www.usenix.org/conference/nsdi24/presentation/zhou-yang), _NSDI '24_
- [**FetchBPF: Customizable Prefetching Policies in Linux with eBPF**](https://www.usenix.org/conference/atc24/presentation/cao), _ATC '24_
- [**eTran: Extensible Kernel Transport with eBPF**](), _NSDI '25_


### Transport Protocol
- [**Data Center TCP (DCTCP)**](https://dl.acm.org/doi/10.1145/1851182.1851192), _SIGCOMM '10_
- [**pFabric: minimal near-optimal datacenter transport**](https://dl.acm.org/doi/10.1145/2486001.2486031), _SIGCOMM '13_
- [**TIMELY: RTT-based Congestion Control for the Datacenter**](https://dl.acm.org/doi/10.1145/2785956.2787510), _SIGCOMM '15_
- [**The QUIC Transport Protocol: Design and Internet-Scale Deployment**](https://dl.acm.org/doi/10.1145/3484266.3487382), _SIGCOMM '17_
- [**Credit-Scheduled Delay-Bounded Congestion Control for Datacenters**](https://dl.acm.org/doi/10.1145/3098822.3098840), _SIGCOMMM '17_
- [**Re-architecting datacenter networks and stacks for low latency and high performance**](https://dl.acm.org/doi/10.1145/3098822.3098825), _SIGCOMMM '17_
- [**Homa: A Receiver-Driven Low-Latency Transport Protocol Using Network Priorities**](https://dl.acm.org/doi/10.1145/3230543.3230564), _SIGCOMMM '18_
- [**HPCC: high precision congestion control**](https://dl.acm.org/doi/10.1145/3341302.3342085), _SIGCOMM '19_
- [**R2P2: Making RPCs first-class datacenter citizens**](https://www.usenix.org/conference/atc19/presentation/kogias-r2p2), _ATC '19_
- [**Swift: Delay is Simple and Effective for Congestion Control in the Datacenter**](https://dl.acm.org/doi/10.1145/3387514.3406591), _SIGCOMM '20_
- [**Aeolus: A Building Block for Proactive Transport in Datacenters**](https://dl.acm.org/doi/10.1145/3387514.3405878), _SIGCOMM '20_
- [**PowerTCP: Pushing the Performance Limits of Datacenter Networks**](https://www.usenix.org/conference/nsdi22/presentation/addanki), _NSDI '21_
- [**TCP is Harmful to In-Network Computing: Designing a Message Transport Protocol (MTP)**](https://dl.acm.org/doi/10.1145/3484266.3487382), _HotNets '21_
- [**Towards Domain-Specific Network Transport for Distributed DNN Training**](https://www.usenix.org/conference/nsdi24/presentation/wang-hao), _NSDI '24_
- [**MTP: A Transport for In-Network Computing**](), _NSDI '25_


### Microservice and Service Mesh
- [**Microservices: yesterday, today, and tomorrow**](https://arxiv.org/pdf/1606.04036.pdf), _Springer '17_
  - One of the first academic papers on microservices. 
- [**Verification in the Age of Microservices**](https://dl.acm.org/doi/10.1145/3102980.3102986), _HotOS '17_
- [**Service Fabric: A Distributed Platform for Building Microservices in the Cloud**](https://dl.acm.org/doi/10.1145/3190508.3190546), _EuroSys '18_
  - A description of the Azure SF design, with a focus on how they solved hard consistency and distributed systems problems.
- [**Overload Control for Scaling WeChat Microservices**](https://dl.acm.org/doi/10.1145/3267809.3267823), _SoCC '18_
- [**µTune: Auto-Tuned Threading for OLDI Microservices**](https://www.usenix.org/conference/osdi18/presentation/sriraman), _OSDI '18_
- [**An Open-Source Benchmark Suite for Microservices and Their Hardware-Software Implications for Cloud & Edge Systems**](https://dl.acm.org/doi/10.1145/3297858.3304013), _ASPLOS '19_
- [**Seer: Leveraging Big Data to Navigate the Complexity of Performance Debugging in Cloud Microservices**](https://dl.acm.org/doi/10.1145/3297858.3304004), _ASPLOS '19_
- [**PARTIES: QoS-Aware Resource Partitioning for Multiple Interactive Services**](https://dl.acm.org/doi/pdf/10.1145/3297858.3304005), _ASPLOS '19_
- [**E3: Energy-Efficient Microservices on SmartNIC-Accelerated Servers**](https://www.usenix.org/conference/atc19/presentation/liu-ming), _ATC '19_
- [**Autopilot: workload autoscaling at Google**](https://dl.acm.org/doi/pdf/10.1145/3342195.3387524), _EuroSys '20_
- [**FIRM: An Intelligent Fine-grained Resource Management Framework for SLO-Oriented Microservices**](https://www.usenix.org/conference/osdi20/presentation/qiu), _OSDI '20_
- [**Accelerometer: Understanding Acceleration Opportunities for Data Center Overheads at Hyperscale**](https://dl.acm.org/doi/10.1145/3373376.3378450), _ASPLOS '20_
  - A study on how microservices spend their CPU cycles. It shows that, within Facebook, microservices spend only a small fraction of their execution time service core application logic, and significant cycles on orchestration work (e.g., compression, serialization, and I/O processing).
- [**Nightcore: Efficient and Scalable Serverless Computing for Latency-Sensitive, Interactive Microservices**](https://dl.acm.org/doi/pdf/10.1145/3445814.3446701), _ASPLOS '21_
- [**Sage: Practical and Scalable ML-Driven Performance Debugging in Microservices**](https://dl.acm.org/doi/pdf/10.1145/3445814.3446700), _ASPLOS '21_
- [**Sinan: ML-Based and QoS-Aware Resource Management for Cloud Microservices**](https://dl.acm.org/doi/pdf/10.1145/3445814.3446693), _ASPLOS '21_
- [**Characterizing Microservice Dependency and Performance: Alibaba Trace Analysis**](https://dl.acm.org/doi/pdf/10.1145/3472883.3487003), _SoCC '21_
- [**SHOWAR: Right-Sizing And Efficient Scheduling of Microservices**](https://dl.acm.org/doi/abs/10.1145/3472883.3486999), _SoCC '21_
- [**Service-Level Fault Injection Testing**](https://dl.acm.org/doi/abs/10.1145/3472883.3487005), _SoCC '21_
- [**Leveraging Service Meshes as a New Network Layer**](https://dl.acm.org/doi/abs/10.1145/3484266.3487379), _HotNets '21_
  - Highlighted service mesh as an abstraction and discussed some use cases and challenges of SM.
- [**SHOWAR: Right-Sizing And Efficient Scheduling of Microservices**](https://dl.acm.org/doi/abs/10.1145/3472883.3486999), _SoCC '21_
- [**DeepRest: Deep Resource Estimation for Interactive Microservices**](https://dl.acm.org/doi/pdf/10.1145/3492321.3519564), _EuroSys '22_
- [**CRISP: Critical Path Analysis of Large-Scale Microservice Architectures**](https://www.usenix.org/conference/atc22/presentation/zhang-zhizhou), _ATC '22_
  - Uber's production-grade microservice tracing system for critical path analysis (CPA), built on top of Jaeger. 
  - Section 7.2 has some interesting data on Uber's microservices in production.
- [**SPRIGHT: Extracting the Server from Serverless Computing! High-performance eBPF-based Event-driven, Shared-memory Processing**](https://dl.acm.org/doi/pdf/10.1145/3544216.3544259), _SIGCOMM '22_
  - Accelerate service mesh (in serverless deployments) using eBPF and shared memory.
- [**DeepScaling: Microservices AutoScaling for Stable CPU Utilization in Large Scale Cloud Systems**](https://dl.acm.org/doi/10.1145/3542929.3563469), _SoCC '22_
- [**The Power of Prediction: Microservice Auto Scaling via Workload Learning**](https://dl.acm.org/doi/10.1145/3542929.3563477), _SoCC '22_
- [**Executing Microservice Applications on Serverless, Correctly**](https://angelhof.github.io/files/papers/mu2sls-2023-popl.pdf), _POPL '23_
- [**The Benefit of Hindsight: Tracing Edge-Cases in Distributed Systems**](https://www.usenix.org/conference/nsdi23/presentation/zhang-lei), _NSDI '23_
- [**Nodens: Enabling Resource Efficient and Fast QoS Recovery of Dynamic Microservice Applications in Datacenters**](https://www.usenix.org/conference/atc23/presentation/shi), _ATC '23_
- [**Lifting the veil on Meta’s microservice architecture: Analyses of topology and request workflows**](https://www.usenix.org/conference/atc23/presentation/huye), _ATC '23_
- [**ServiceRouter: Hyperscale and Minimal Cost Service Mesh at Meta**](https://www.usenix.org/conference/osdi23/presentation/saokar), _OSDI '23_
- [**Network-Centric Distributed Tracing with DeepFlow: Troubleshooting Your Microservices in Zero Code**](https://dl.acm.org/doi/10.1145/3603269.3604823), _SIGCOMM '23_
- [**Dissecting Overheads of Service Mesh Sidecars**](https://dl.acm.org/doi/10.1145/3620678.3624652), _SoCC '23_
- [**LatenSeer: Causal Modeling of End-to-End Latency Distributions by Harnessing Distributed Tracing**](https://dl.acm.org/doi/10.1145/3620678.3624787), _SoCC '23_
- [**Expressive Policies For Microservice Networks**](https://dl.acm.org/doi/10.1145/3626111.3628181), _HotNets '23_
  - Language and system support for complex safety properties that reason about the flow of requests across the whole microservice network (not just between adjacent hops).  
- [**Application Defined Networks**](https://dl.acm.org/doi/10.1145/3626111.3628178), _HotNets '23_
- [**Cilantro: Performance-Aware Resource Allocation for General Objectives via Online Feedback**](https://www.usenix.org/conference/osdi23/presentation/bhardwaj), _OSDI '23_
- [**Blueprint: A Toolchain for Highly-Reconfigurable Microservice Applications**](https://dl.acm.org/doi/10.1145/3600006.3613138), _SOSP '23_
- [**MuCache: a General Framework for Caching in Microservice Graphs**](https://www.usenix.org/conference/nsdi24/presentation/zhang-haoran), _NSDI '24_
- [**Autothrottle: A Practical Bi-Level Approach to Resource Management for SLO-Targeted Microservices**](https://www.usenix.org/conference/nsdi24/presentation/wang-zibo), _NSDI '24_
- [**TraceWeaver: Distributed Request Tracing for Microservices Without Application Modification**](https://dl.acm.org/doi/10.1145/3651890.3672254), _SIGCOMM '24_
- [**TopFull: An Adaptive Top-Down Overload Control for SLO-Oriented Microservices**](https://dl.acm.org/doi/10.1145/3651890.3672253), __SIGCOMM '24_
- [**Canal Mesh: A Cloud-Scale Sidecar-Free Multi-Tenant Service Mesh Architecture**](https://dl.acm.org/doi/10.1145/3651890.3672221), __SIGCOMM '24_
- [**Derm: SLA-aware Resource Management for Highly Dynamic Microservices**](https://ieeexplore.ieee.org/abstract/document/10609698), __ISCA '24_

### Network Stack and RPC 
- [**netmap: A Novel Framework for Fast Packet I/O**](https://www.usenix.org/conference/atc12/technical-sessions/presentation/rizzo), _ATC '12_
- [**Chronos: Predictable Low Latency for Data Center Applications**](https://dl.acm.org/doi/10.1145/2391229.2391238), _SoCC'12_
- [**Improving Network Connection Locality on Multicore Systems**](https://dl.acm.org/doi/10.1145/2168836.2168870), _EuroSys'12_
- [**MegaPipe: A New Programming Interface for Scalable Network I/O**](https://www.usenix.org/conference/osdi12/technical-sessions/presentation/han), _OSDI'12_
- [**mTCP: a Highly Scalable User-level TCP Stack for Multicore Systems**](https://www.usenix.org/conference/nsdi14/technical-sessions/presentation/jeong), _NSDI '14_
- [**Network stack specialization for performance**](https://dl.acm.org/doi/10.1145/2619239.2626311), _SIGCOMM '14_
- [**IX: A Protected Dataplane Operating System for High Throughput and Low Latency**](https://www.usenix.org/conference/osdi14/technical-sessions/presentation/belay), _OSDI '14_
- [**Arrakis: The Operating System is the Control Plane**](https://www.usenix.org/conference/osdi14/technical-sessions/presentation/peter), _OSDI '14_
- [**StackMap: Low-Latency Networking with the OS Stack and Dedicated NICs**](https://www.usenix.org/conference/atc16/technical-sessions/presentation/yasukata), _ATC '16_
- [**ModNet: A Modular Approach to Network Stack Extension**](https://www.usenix.org/conference/nsdi15/technical-sessions/presentation/pathak), _NSDI '15_
- [**RSS++: load and state-aware receive side scaling**](https://dl.acm.org/doi/10.1145/3359989.3365412), _CoNEXT '19_
- [**TAS: TCP Acceleration as an OS Service**](https://dl.acm.org/doi/10.1145/3302424.3303985), _EuroSys '19_
  - Accelates TCP stack by splitting the stack into a "fast" data path (for data transport of established connections) and a control plane (for connection and context management, congestion control etc.).
- [**Snap: a Microkernel Approach to Host Networking**](https://dl.acm.org/doi/10.1145/3341301.3359657), _SOSP '19_
- [**SocksDirect: Datacenter Sockets can be Fast and Compatible**](https://dl.acm.org/doi/10.1145/3341302.3342071), _SIGCOMM '19_
- [**Understanding Host Network Stack Overheads**](https://dl.acm.org/doi/abs/10.1145/3452296.3472888), _SIGCOMM '20_
- [**The nanoPU: A Nanosecond Network Stack for Datacenters**](https://www.usenix.org/conference/osdi21/presentation/ibanez), _OSDI '21_
- [**How to diagnose nanosecond network latencies in rich end-host stacks**](https://www.usenix.org/conference/nsdi22/presentation/haecki), _NSDI '22_
- [**Remote Procedure Call as a Managed System Service**](https://www.usenix.org/conference/nsdi23/presentation/chen-jingrong), _NSDI '23_
- [**NetClone: Fast, Scalable, and Dynamic Request Cloning for Microsecond-Scale RPCs**](https://dl.acm.org/doi/10.1145/3603269.3604820), _SIGCOMM '23_
- [**Fathom: Understanding Datacenter Application Network Performance**](https://dl.acm.org/doi/pdf/10.1145/3603269.3604815), _SIGCOMM '23_
- [**A Cloud-Scale Characterization of Remote Procedure Calls**](https://dl.acm.org/doi/10.1145/3600006.3613156), _SOSP '23_
- [**HydraRPC: RPC in the CXL Era**](https://www.usenix.org/conference/atc24/presentation/ma), _ATC '24_

### Workload Interference
- [**Q-Clouds: Managing Performance Interference Effects for QoS-Aware Clouds**](https://dl.acm.org/doi/abs/10.1145/1755913.1755938), _EuroSys '10_
  - Profiling applications' performance in a standalone mode and using that to provide a baseline target when consolidating them onto a shared host.  
- [**Cuanta: quantifying effects of shared on-chip resource interference for consolidated virtual machines**](https://dl.acm.org/doi/10.1145/2038916.2038938), _SoCC '11_
  - Introduced a cache loader micro-benchmark to profile application performance under varying cache-usage pressure and use the profile to predict the impact of cache interference among consolidated workloads  
- [**Bubble-up: Increasing utilization in modern warehouse scale computers via sensible co-locations**](https://ieeexplore.ieee.org/document/7851476), _MICRO '11_
  - Each application is profiled 1) using a memory antagonist to obtain its (memory) sensitivity curve and 2) to measure the pressure on the memory it generates.  
- [**Toward Predictable Performance in Software Packet-Processing Platforms**](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/dobrescu), _NSDI '12_
  - Profile each NF’s cache ref/sec running alone and its performance drop curve when collocating with a synthetic antagonist. Predict the performance drop with these profiles. 
 - [**DeepDive: Transparently Identifying and Managing Performance Interference in Virtualized Environments**](https://www.usenix.org/conference/atc13/technical-sessions/presentation/novakovi), _ATC '13_
  - Detect interference via differential low-level metrics (see Table 1), validate the interference and identify the interfering resource by running the victim in isolation, and mitigate interference via migration. 
- [**Bobtail: Avoiding Long Tails in the Cloud**](https://www.usenix.org/conference/nsdi13/technical-sessions/presentation/xu_yunjing), _NSDI '13_
- [**Paragon: QoS-Aware Scheduling for Heterogeneous Datacenters**](https://dl.acm.org/doi/10.1145/2451116.2451125), _ASPLOS '13_
- [**CPI2 : CPU performance isolation for shared compute clusters**](https://dl.acm.org/doi/10.1145/2465351.2465388), _EuroSys '13_
  - Uses cycles-per-instruction (CPI) as metrics to detect workload interference and identify perpetrators (and address the interference by throttling). Key takeaway: CPI correlates with application performance and CPI is a stable metrics.   
- [**Reconciling High Server Utilization and Sub-millisecond Quality-of-Service**](https://dl.acm.org/doi/10.1145/2592798.2592821), _EuroSys '14_
  - Co-location leads to increases in queuing delay, scheduling delay, and thread load imbalance. Addresses interference online via re-provisioning and scheduling.
- [**Heracles: Improving resource efficiency at scale**](https://ieeexplore.ieee.org/document/7284086), _ISCA '15_
  - Manage workload (LC+BE) colocations via an online controller that monitors latency and resource usage and manages the isolation mechanism for different resources.
- [**PerfIso: Performance Isolation for Commercial Latency-Sensitive Services**](https://www.usenix.org/conference/atc18/presentation/iorgulescu), _ATC '18_
  - Described a production system (Microsoft Bing) for performance isolation  
- [**PARTIES: QoS-Aware Resource Partitioning for Multiple Interactive Services**](https://dl.acm.org/doi/10.1145/3297858.3304005), _ASPLOS '19_ 
  - Online monitoring that detects QoS violations in O(100ms) and boosts the resource allocation of victims.  
- [**PicNIC: predictable virtualized NIC**](https://dl.acm.org/doi/10.1145/3341302.3342093), _SIGCOMM '19_
  - Characterize how performance isolation can break in virtualized network stack in terms of network bandwidth and network stack processing rate. Provides an abstraction and construct based on bandwidth, latency, and loss rate to detect isolation breakdown and enforce isolation.  
- [**Shenango: Achieving High CPU Efficiency for Latency-sensitive Datacenter Workloads**](https://www.usenix.org/conference/nsdi19/presentation/ousterhout), _NSDI '19_
- [**Caladan: Mitigating Interference at Microsecond Timescales**](https://www.usenix.org/conference/osdi20/presentation/fried), _OSDI '20_
  - Uses a set of control signals and corresponding actions to detect and respond to interference over microsecond timescales.  
- [**FIRM: An Intelligent Fine-Grained Resource Management Framework for SLO-Oriented Microservices**](https://www.usenix.org/conference/osdi20/presentation/qiu), _OSDI '20_
  - Use online telemetry data (resource usage and latency) and offline learned models to detect and localize microservices that cause SLO violations and mitigate violations via dynamic re-provisioning.


### Network Architecture
- [**Architectural considerations for a new generation of protocols**](https://dl.acm.org/doi/10.1145/99517.99553), _SIGCOMM CCR '90_
- [**A Data-Oriented (and Beyond) Network Architecture**](https://dl.acm.org/doi/pdf/10.1145/1282380.1282402), _SIGCOMM '07_
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
- [**Houdini's Escape: Breaking the Resource Rein of Linux Control Groups**](https://dl.acm.org/doi/10.1145/3319535.3354227), _CCS '19_
- [**Particle: Ephemeral Endpoints for Serverless Networking**](https://dl.acm.org/doi/10.1145/3419111.3421275), _SoCC '20_
- [**Parallelizing packet processing in container overlay networks**](https://dl.acm.org/doi/10.1145/3447786.3456241), _EuroSys '21_
- [**MigrOS: Transparent Live-Migration Support for Containerised RDMA Applications**](https://www.usenix.org/conference/atc21/presentation/planeta), _ATC '21_
- [**Starlight: Fast Container Provisioning on the Edge and over the WAN**](https://www.usenix.org/conference/nsdi22/presentation/chen-jun-lin), _NSDI '22_
- [**Transparent GPU Sharing in Container Clouds for Deep Learning Workloads**](https://www.usenix.org/conference/nsdi23/presentation/wu), _NSDI '23_


