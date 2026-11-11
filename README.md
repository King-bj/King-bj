# Hi, I'm King

I started as a Java developer in 2016, took responsibility for operations platform development in November 2019, and began operating production Kubernetes environments in 2024.

My work has included deploying an operations platform on Kubernetes, integrating SkyWalking probes, and building cluster diagnostics with RBAC-scoped access. When an application team needed tracing without an in-process agent, I evaluated eBPF collection and tested its limits on ARM64. On Kylin V10 SP3 with kernel 4.19, we verified the HTTP/1.x request path end to end.

## Selected engineering notes

- [Why Kubernetes replicas generated duplicate IDs](https://docs.jinla.fun/posts/k8s-id) — how moving from VMs to pods changed instance identity, and where a hash-based workaround can still collide.
- [Sizing a monitoring and logging platform](https://docs.jinla.fun/posts/ops-cap) — a worked example that estimates ingestion rates and identifies which measurements to collect before scaling.

## Code sample

[Notify Hub's notification dispatcher](https://github.com/King-bj/rc_jinla/blob/main/src/main/java/com/notifyhub/dispatcher/NotificationDispatcher.java) is part of a small interview project. It shows how I schedule HTTP deliveries, retry failed attempts and record exhausted tasks. A successful remote call followed by a failed local commit can still result in a repeat delivery.

[Engineering blog](https://docs.jinla.fun/) · [Contact me](mailto:jlnwcy@gmail.com)
