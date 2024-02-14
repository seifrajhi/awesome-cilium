# Awesome Cilium [![Awesome](https://awesome.re/badge.svg)](https://github.com/sindresorhus/awesome)

> Cilium is an open-source networking project that provides networking and security capabilities for containerized applications, microservices, and virtual machines. 


> Recently [Cilium](https://docs.cilium.io/en/stable) launched a great website about eBPF called [ebpf.io](https://ebpf.io/). It serves a similar purpose to this list, with [an introduction to eBPF](https://ebpf.io/what-is-ebpf).

> Note: Cilium is an exciting piece of technology, and its ecosystem is constantly evolving. We'd love help from _you_ to keep this awesome list up to date, and improve its signal-to-noise ratio in anyway we can. Please feel free to leave [any feedback](https://github.com/seifrajhi/awesome-cilium/issues).

## Contents

- [Reference Documentation](#reference-documentation)
- [Cilium related projects](#cilium-related-projects)
- [Articles and Presentations](#articles-and-presentations)
- [Community Events](#community-events)
- [Community and Contributing](#community-and-contributing)
- [Hands on Contents](#hands-on-contents)

## Reference Documentation

- [Website](https://cilium.io) - Official website of cilium which was originally created by [Isovalent](https://isovalent.com/).

- [Official GitHub repository](https://github.com/cilium) - GitHub Repository of cilium project.

- [A cookbook of installing cilium on AWS EKS](https://github.com/littlejo/cilium-eks-cookbook) - Multiple ways to install cilium in eks.

- [Cilium Certified Associate Study Guide](https://github.com/isovalent/CCA-Study-Guide) - Study guide  to help the Cilium community prepare for the CNCF's Cilium Certified Associate(CCA) Exam.

## Cilium related projects

- [Cilium](https://github.com/cilium/cilium) - The core project, Cilium, is a networking plugin for various container runtimes such as Kubernetes, Docker, and Mesos. It leverages Linux kernel features like eBPF (extended Berkeley Packet Filter) to provide fast and secure networking and load balancing for applications.

- [eBPF](https://github.com/cilium/ebpf) - Extended Berkeley Packet Filter (eBPF) is a technology that allows for dynamic, programmable packet filtering and network analysis in the Linux kernel. Cilium heavily relies on eBPF to enhance the networking and security capabilities of containerized applications.

- [Cilium Proxy](https://github.com/cilium/proxy) - Cilium Proxy is a high-performance HTTP, TCP, and gRPC proxy that can be automatically injected into Kubernetes pods. It provides features like load balancing, health checking, and L7 (Layer 7) visibility, helping secure and monitor application traffic.

- [Cilium Cluster Mesh](https://docs.cilium.io/en/v1.9/gettingstarted/clustermesh/) - Cilium Cluster Mesh allows you to securely connect multiple Kubernetes clusters together using encrypted tunnels. It enables seamless communication and service discovery across clusters while maintaining strong security boundaries.

- [Hubble](https://github.com/cilium/hubble) - Hubble is a network visibility and monitoring tool built by the Cilium community. It provides real-time visibility into network traffic, allowing operators to gain insights into application behavior, troubleshoot connectivity issues, and enforce network security policies.

- [Cilium Operator](https://docs.cilium.io/en/stable/internals/cilium_operator/) - Cilium Operator is a Kubernetes operator that simplifies the deployment and management of Cilium within a Kubernetes cluster. It automates tasks such as deploying Cilium agents, configuring eBPF policies, and handling upgrades.

- [Tetragon](https://github.com/cilium/tetragon) - Tetragon is a runtime security enforcement and observability tool.

- [Cilium Mesh](https://isovalent.com/blog/post/introducing-cilium-mesh/) - Cilium Mesh connects Kubernetes workloads, virtual machines, and physical servers running in the cloud, on-premises, or at the edge.

- [NetworkPolicy Editor](https://editor.networkpolicy.io/) - Create, Visualize, and Share Kubernetes NetworkPolicies.

- [Prometheus & Grafana for Cilium](https://github.com/cilium/cilium/tree/main/examples/kubernetes/addons/prometheus) - Collect metrics from Cilium and store them in Prometheus for analysis and alerting.

- [Cilium Helm Chart](https://artifacthub.io/packages/helm/cilium/cilium) - Helm chart that can be used to deploy Cilium on Kubernetes.

- [Hubble adaptor for OpenTelemetry](https://github.com/cilium/hubble-otel) - Enable exporting Hubble flow data using OpenTelemetry collector.

- [Packet, where are you?](https://github.com/cilium/pwru) - eBPF-based Linux kernel networking debugger.

- [Coroot](https://github.com/coroot/coroot) - It  turns telemetry data into actionable insights, helping you identify and resolve application issues quickly.

- [Pixie](https://github.com/pixie-io/pixie) - Instant Kubernetes-Native Application Observability.

- [caretta](https://github.com/groundcover-com/caretta) - Instant K8s service dependency map, right to your Grafana.

- [Gloo Network](https://www.solo.io/products/gloo-network/) - Gloo Network enables Cilium-CNI powered by eBPF to enable networking, packet filtering and observability for modern applications.


- [Bpfilter instead of iptables for routing](https://www.admin-magazine.com/Archive/2019/50/Bpfilter-offers-a-new-approach-to-packet-filtering-in-Linux) - Bpfilter offers a new approach to packet filtering in Linux.
  

![image](https://github.com/seifrajhi/awesome-cilium/assets/26981510/b2236520-ea4c-400d-a5fd-15850a8bf420)


- [Inter-node traffic control](https://docs.cilium.io/en/latest/network/kubernetes/policy/#ciliumclusterwidenetworkpolicy) - Policies that are applicable to the whole cluster (non-namespaced) and provide you with the means to specify nodes as the source and target.


- [BPF and XDP Reference Guide](http://docs.cilium.io/en/latest/bpf/) - Guide from the Cilium project.

- [Why is the kernel community replacing iptables with BPF?](https://cilium.io/blog/2018/04/17/why-is-the-kernel-community-replacing-iptables/) - A blog post by Cilium on the the motivations behind eBPF and bpfilter, with a couple examples and links to other projects using eBPF and bpfilter.

- [Bpfilter: Linux firewall with eBPF sauce](https://qmo.fr/docs/talk_20180316_frnog_bpfilter.pdf) - Slides from a talk by Quentin Monnet with a background on eBPF and comparing bpfilter to iptables.

- [Cilium: Networking & Security for Containers with BPF & XDP](http://www.slideshare.net/ThomasGraf5/clium-container-networking-with-bpf-xdp) - Also featuring a load balancer use case.

- [Cilium: Networking & Security for Containers with BPF & XDP](http://www.slideshare.net/Docker/cilium-bpf-xdp-for-containers-66969823) - [video](https://www.youtube.com/watch?v=TnJF7ht3ZYc&list=PLkA60AVN3hh8oPas3cq2VA9xB7WazcIgs).

- [Cilium: Fast IPv6 container Networking with BPF and XDP](http://www.slideshare.net/ThomasGraf5/cilium-fast-ipv6-container-networking-with-bpf-and-xdp) - Fast IPv6 container Networking with BPF and XDP.

- [Cilium: BPF & XDP for containers](https://fosdem.org/2017/schedule/event/cilium/) - PF & XDP for containers.

- [Learning ebpf book](https://github.com/lizrice/learning-ebpf) - Learning eBPF, published by O'Reilly! Here's where you will find a VM config for the examples.

## Articles and Presentations

- [eBPF log analytics in your Kubernetes cluster](https://www.parseable.io/blog/ebpf-log-analytics) - Leverage Cilium's Tetragon to capture eBPF based file access logs and send it to Parseable for alerting and further analytics.

- [Introduction to Cilium](https://www.youtube.com/watch?v=80OYrzS1dCA) - A livestream covering all things related to eBPF and Cilium presented by Isovalent's Thomas Graf & Liz Rice. 


- [Cilium CNI](https://medium.com/itnext/cilium-cni-a-comprehensive-deep-dive-guide-for-networking-and-security-enthusiasts-588afbf72d5c) - A Comprehensive Deep Dive Guide for Networking and Security Enthusiasts.

- [Cilium for Kubernetes networking](https://blog.palark.com/why-cilium-for-kubernetes-networking/) - Why we use it and why we love it.

- [A generic introduction to Cilium](https://opensource.googleblog.com/2016/11/cilium-networking-and-security.html) - A generic introduction to Cilium.

- [A podcast interviewing Thomas Graf](http://blog.ipspace.net/2016/10/fast-linux-packet-forwarding-with.html) - Ivan Pepelnjak interviewing Thomas, October 2016, on eBPF, P4, XDP and Cilium.

- [How eBPF Streamlines the Service Mesh](https://thenewstack.io/how-ebpf-streamlines-the-service-mesh/) - Explore how eBPF allows us to streamline the service mesh, making the data plane more efficient and easier to deploy.

- [From Amazon VPC CNI to Cilium with Zero Downtime](https://medium.com/codex/migrate-to-cilium-from-amazon-vpc-cni-with-zero-downtime-493827c6b45e) - Migrate to Cilium from Amazon VPC CNI with Zero Downtime. 

- [Cilium CNI and OKE on Oracle Cloud](https://medium.com/oracledevs/cni-adventures-with-kubernetes-on-oracle-cloud-cilium-5c6f011746d5) - Kubernetes Networking with Cilium CNI and OKE on Oracle Cloud.

- [Cilium in Azure Kubernetes Service (AKS)](https://learn.microsoft.com/en-us/azure/aks/azure-cni-powered-by-cilium) - Configure Azure CNI Powered by Cilium in Azure Kubernetes Service (AKS).

- [eCHO News NEWSLETTER](https://www.linkedin.com/newsletters/echo-news-6937495018668482560/) - eCHO news in a bi-weekly wrap up of all things eBPF and Cilium.

- [Exploring eBPF and XDP](https://naftalyava.com/example-xdp-ebpf-code-for-handling-ingress-traffic/) - An Example - A basic example how to get started with XDP.

- [eBPF - Rethinking the Linux Kernel](https://docs.google.com/presentation/d/1AcB4x7JCWET0ysDr0gsX-EIdQSTyBtmi6OAW7bE0jm0/edit#slide=id.g6e43ab8f8d_0_612) - eBPF JavaScript-like capabilities to the Linux Kernel.

- [Learn how Tetragon can stop CVEs with YAML](https://djalal.opendz.org/post/prevent-kernel-overlayfs-ubuntu-cves-with-yaml/) - Prevent Overlayfs Privilege Escalation on Ubuntu Kernels with Yaml (bpf).

- [Cilium + Istio](https://www.solo.io/blog/cilium-1-14-istio/) - A Quick Tour of Cilium 1.14 with Istio.

- [Cilium: Decoding the packet path with Security Groups for Pods in EKS](https://medium.com/@amitmavgupta/security-groups-for-pods-in-eks-cilium-and-networking-f809cf72fc31) - Decoding the packet path with Security Groups for Pods in EKS.

- [Cilium mutual auth … DIY](https://xxradar.medium.com/cilium-mutual-auth-diy-5d5036a82cf9) - A quick run-through on setting up cilium, mtls on a self-managed kubernetes cluster.
  
- [Istio Service Mesh with ALB in EKS](https://medium.com/@amitmavgupta/installing-cilium-in-azure-kubernetes-service-byocni-with-no-kube-proxy-825b9007b24b) - Install Cilium in a BYOCNI mode seamlessly and thus leverage #ebpf functionality as compared to iptables.

- [Kubernetes LoadBalance service using Cilium BGP control plane](https://medium.com/@valentin.hristev/kubernetes-loadbalance-service-using-cilium-bgp-control-plane-8a5ad416546a) - A walk through the process of creating Cilium based support for Load Balancer Services in a minimal K3s Kubernetes cluster.

- [eBPF-based networking with Cilium](https://b-nova.com/en/home/content/ebpf-based-networking-with-cilium) - What is it and what can it do?.

- [Deploying Red Hat OpenShift with Cilium](https://isovalent.com/blog/post/deploying-red-hat-openshift-with-cilium/) - Given that OpenShift is pretty ubiquitous in private clouds (especially in financial organizations) and that Cilium is on its way to become ubiquitous, this tutorial on deploying Cilium and Red Hat OpenShift will be handy for many.

- [Setting up EKS Amazon Clusters, adding Cilium to projects using Terraform and Helm, supporting GitOps, and using Karpenter for efficient resource utilization and cost savings](https://aws.plainenglish.io/architecting-for-resilience-crafting-opinionated-eks-clusters-with-karpenter-cilium-cluster-mesh-c87cee1df934) - Architecting for Resilience: Crafting Opinionated EKS Clusters with Karpenter & Cilium Cluster Mesh.

- [Kubernetes Gateway API with Cilium](https://kubito.dev/posts/kubernetes-gateway-api-cilium/) - This article provides guidance on how to effectively configure Cilium for setting up the Gateway API in Kubernetes environments.

- [How to migrate from Red Hat OpenShiftSDN/OVN-Kubernetes to Cilium](https://veducate.co.uk/migrate-red-hat-openshiftsdn-ovn-kubernetes-cilium/) - A step-by-step process of migrating from the traditional OpenShiftSDN (default CNI pre-4.12) or OVN-Kubernetes (default CNI from 4.12) to Cilium, exploring the advantages and considerations along the way.

- [Setup basic L4 Load Balancing with Cilium CNI and Ubuiqiti Edge Router](https://www.viktorious.nl/2024/01/05/setup-basic-l4-load-balancing-with-cilium-cni-and-ubuiqiti-edge-router/) - Setting up basic L4 Load Balancing with Cilium CNI and Ubuiqiti Edge Router.

## Community Events

- [CiliumCon](https://cilium.io/events/) - CiliumCon is a full-day co-located event for Cilium users, contributors, and new community members.

- [Isovalent Security Summer School 2023](https://isovalent.com/events/2023-07-security-summer-school/) - Virtual Security Summer School where you can level up your skills with hands-on labs. Learn how Cilium, Tetragon, and Hubble help improve Kubernetes security.

- [Isovalent's cilium related events](https://isovalent.com/events/) - Events featuring diverse voices, innovative companies and big ideas.

## Community and Contributing

- [Slack channel](https://cilium.herokuapp.com/) - For live conversation and quick questions, join the Cilium Slack workspace.

- [Twitter](https://twitter.com/ciliumproject) - Follow Cilium on Twitter for the latest news and announcements.
  
- [YouTube](https://www.youtube.com/c/eBPFCiliumCommunity) - Watch the videos from the Cilium and eBPF Communities.
  
- [Contributors](https://github.com/cilium/cilium/graphs/contributors) - Contributions to main.

## Hands on Contents

- [Isovalent library for Cilium](https://isovalent.com/resource-library/) - You can find Videos `Case studies`, `Blogs`, `Books`, `Labs` and `Analyst Reports`.

- [Cilium Learning Tracks](https://isovalent.com/learning-tracks/) - Pick from tracks for cloud network engineers, security professionals, platform engineers, platform ops (service mesh), and cloud architects.

- [K0S Cilium Playground](https://github.com/xinity/k0s_cilium_playground) - A full bash based k0s Cilium Clustermesh enabled playground.

- [Podcast: Kubernetes Unpacked Podcast](https://packetpushers.net/podcast/kubernetes-unpacked-022-kubernetes-networking-and-abstraction-with-cilium-and-ebpf/) - Kubernetes Unpacked 022: Kubernetes Networking And Abstraction With Cilium And eBPF.

- [From Zero to Cluster Mesh: Installing and Configuring Cilium CNI on Kubernetes](https://www.youtube.com/watch?v=z8Kifl3M3LU&list=PLQpKr4_0p0jEIGtCeV4VcGd_-Jf49e1JY) - How to install and configure the Cilium CNI (Container Network Interface) and enable its advanced cluster mesh feature across Kubernetes clusters in different availability zones!.

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

