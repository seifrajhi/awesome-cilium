# Awesome Cilium [![Awesome](https://awesome.re/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of awesome projects related to Cilium.

Cilium is an open-source networking project that provides networking and security capabilities for containerized applications, microservices, and virtual machines. 


Recently [Cilium](https://cilium.io) launched a great website about eBPF called [ebpf.io](https://ebpf.io/). It serves a similar purpose to this list, with [an introduction to eBPF](https://ebpf.io/what-is-ebpf).

> Note: Cilium is an exciting piece of technology, and its ecosystem is constantly evolving. We'd love help from _you_ to keep this awesome list up to date, and improve its signal-to-noise ratio in anyway we can. Please feel free to leave [any feedback](https://github.com/seifrajhi/awesome-cilium/issues).

Here are some notable projects and concepts related to Cilium:



## Contents

- [Reference Documentation](#reference-documentation)
- [Articles and Presentations](#articles-and-presentations)
- [Community Events](community-events)
- [Community and Contributing](#community-and-contributing)



## Reference Documentation

- [Official website](https://cilium.io/) of cilium which was originally created by [Isovalent](https://isovalent.com/)

- [Official github repository](https://github.com/cilium): of cilium project.

### Cilium related projects

- [Cilium](https://github.com/cilium/cilium): The core project, Cilium, is a networking plugin for various container runtimes such as Kubernetes, Docker, and Mesos. It leverages Linux kernel features like eBPF (extended Berkeley Packet Filter) to provide fast and secure networking and load balancing for applications.

- [eBPF](https://github.com/cilium/ebpf): Extended Berkeley Packet Filter (eBPF) is a technology that allows for dynamic, programmable packet filtering and network analysis in the Linux kernel. Cilium heavily relies on eBPF to enhance the networking and security capabilities of containerized applications.

- [Cilium Proxy](https://github.com/cilium/proxy): Cilium Proxy is a high-performance HTTP, TCP, and gRPC proxy that can be automatically injected into Kubernetes pods. It provides features like load balancing, health checking, and L7 (Layer 7) visibility, helping secure and monitor application traffic.

- [Cilium Cluster Mesh](https://docs.cilium.io/en/v1.9/gettingstarted/clustermesh/): Cilium Cluster Mesh allows you to securely connect multiple Kubernetes clusters together using encrypted tunnels. It enables seamless communication and service discovery across clusters while maintaining strong security boundaries.

- [Hubble](https://github.com/cilium/hubble): Hubble is a network visibility and monitoring tool built by the Cilium community. It provides real-time visibility into network traffic, allowing operators to gain insights into application behavior, troubleshoot connectivity issues, and enforce network security policies.

- [Cilium Operator](https://docs.cilium.io/en/stable/internals/cilium_operator/): Cilium Operator is a Kubernetes operator that simplifies the deployment and management of Cilium within a Kubernetes cluster. It automates tasks such as deploying Cilium agents, configuring eBPF policies, and handling upgrades.

- [Tetragon](https://github.com/cilium/tetragon): Tetragon is a runtime security enforcement and observability tool. 

- [Cilium Mesh](https://isovalent.com/blog/post/introducing-cilium-mesh/): Cilium Mesh connects Kubernetes workloads, virtual machines, and physical servers running in the cloud, on-premises, or at the edge.

- [NetworkPolicy Editor](https://editor.networkpolicy.io/): Create, Visualize, and Share Kubernetes NetworkPolicies.

- [Prometheus & Grafana for Cilium](https://github.com/cilium/cilium/tree/main/examples/kubernetes/addons/prometheus): Collect metrics from Cilium and store them in Prometheus for analysis and alerting.

- [Cilium Helm Chart](https://artifacthub.io/packages/helm/cilium/cilium): Helm chart that can be used to deploy Cilium on Kubernetes.

- [Hubble adaptor for OpenTelemetry](https://github.com/cilium/hubble-otel): Enable exporting Hubble flow data using OpenTelemetry collector.

- [Bpfilter instead of iptables for routing](https://www.admin-magazine.com/Archive/2019/50/Bpfilter-offers-a-new-approach-to-packet-filtering-in-Linux): Bpfilter offers a new approach to packet filtering in Linux.

![image](https://github.com/seifrajhi/awesome-cilium/assets/26981510/b2236520-ea4c-400d-a5fd-15850a8bf420)


- [Inter-node traffic control](https://docs.cilium.io/en/latest/network/kubernetes/policy/#ciliumclusterwidenetworkpolicy): Policies that are applicable to the whole cluster (non-namespaced) and provide you with the means to specify nodes as the source and target.


- [BPF and XDP Reference Guide](http://docs.cilium.io/en/latest/bpf/): - Guide from the Cilium project.

- [Why is the kernel community replacing iptables with BPF?](https://cilium.io/blog/2018/04/17/why-is-the-kernel-community-replacing-iptables/) - A blog post by Cilium on the the motivations behind eBPF and bpfilter, with a couple examples and links to other projects using eBPF and bpfilter.

- [bpfilter: Linux firewall with eBPF sauce](https://qmo.fr/docs/talk_20180316_frnog_bpfilter.pdf): - Slides from a talk by Quentin Monnet with a background on eBPF and comparing bpfilter to iptables.

- [Cilium: Networking & Security for Containers with BPF & XDP](http://www.slideshare.net/ThomasGraf5/clium-container-networking-with-bpf-xdp) - Also featuring a load balancer use case

- [Cilium: Networking & Security for Containers with BPF & XDP](http://www.slideshare.net/Docker/cilium-bpf-xdp-for-containers-66969823) - [video](https://www.youtube.com/watch?v=TnJF7ht3ZYc&list=PLkA60AVN3hh8oPas3cq2VA9xB7WazcIgs)

- [Cilium: Fast IPv6 container Networking with BPF and XDP](http://www.slideshare.net/ThomasGraf5/cilium-fast-ipv6-container-networking-with-bpf-and-xdp)

- [Cilium: BPF & XDP for containers](https://fosdem.org/2017/schedule/event/cilium/)

## Articles and Presentations

- [Introduction to Cilium](https://www.youtube.com/watch?v=80OYrzS1dCA): A livestream covering all things related to eBPF and Cilium presented by Isovalent's Thomas Graf & Liz Rice. 


- [Cilium CNI](https://medium.com/itnext/cilium-cni-a-comprehensive-deep-dive-guide-for-networking-and-security-enthusiasts-588afbf72d5c): A Comprehensive Deep Dive Guide for Networking and Security Enthusiasts!

- [Cilium for Kubernetes networking](https://blog.palark.com/why-cilium-for-kubernetes-networking/): Why we use it and why we love it

- [A generic introduction to Cilium](https://opensource.googleblog.com/2016/11/cilium-networking-and-security.html)

- [A podcast interviewing Thomas Graf](http://blog.ipspace.net/2016/10/fast-linux-packet-forwarding-with.html) - Ivan Pepelnjak interviewing Thomas, October 2016, on eBPF, P4, XDP and Cilium.

- [How eBPF Streamlines the Service Mesh](https://thenewstack.io/how-ebpf-streamlines-the-service-mesh/): Explore how eBPF allows us to streamline the service mesh, making the data plane more efficient and easier to deploy. 

## Community Events

- [CiliumCon](https://cilium.io/events/): CiliumCon is a full-day co-located event for Cilium users, contributors, and new community members.

- [Isovalent Security Summer School 2023](https://isovalent.com/events/2023-07-security-summer-school/): Virtual Security Summer School where you can level up your skills with hands-on labs. Learn how Cilium, Tetragon, and Hubble help improve Kubernetes security.

## Community and Contributing

- [Slack channel](https://cilium.herokuapp.com/): For live conversation and quick questions, join the Cilium Slack workspace

- [Twitter](https://twitter.com/ciliumproject): Follow Cilium on Twitter for the latest news and announcements.
  
- [YouTube](https://www.youtube.com/c/eBPFCiliumCommunity): Watch the videos from the Cilium and eBPF Communities.
  
- [Contributors](https://github.com/cilium/cilium/graphs/contributors): Contributions to main.


## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, rajhiseif has waived all copyright and related or neighboring rights to this work.
