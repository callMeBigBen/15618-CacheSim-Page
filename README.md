# 15618 Multi-Core Cache Simulator

## Links
- See [here](#) for the proposal.
- [This](#) is the link to the project website.
- [This](#) is the link to the project repository.

## Summary
We are going to implement a trace-driven multicore cache simulator supporting both snooping and directory based cache coherence protocols. We further want to perform workload analysis for program with different access patterns, locality, sharing, and the effect of different interconnect topologies on cache performance.

## Backgroud
We studied multiple cache coherence protocols during the lectures such as MSI, MESI, and MOESI. We also studied a couple of different implementation styles namely snooping-based and directory-based. We are curious about the practical implications and their effect on the performance of a multi-core cache system. 

We're excited about studying the effect of different sizes of a cache line and replacement policies, on the performance of the multi-core cache system.

State diagram for MESI:
<img width="1158" alt="image" src="https://user-images.githubusercontent.com/33094628/200696776-cc0c2505-8d7b-4f26-92ec-3ca07d6350d6.png">

Design of snooping-based cache coherence:
![image](https://user-images.githubusercontent.com/33094628/200697282-c4613b3b-0588-445b-9bd4-f1580f2476eb.png)

Design of directory-based cache coherence:
<img width="1063" alt="image" src="https://user-images.githubusercontent.com/33094628/200697445-d9e84f6f-7699-4a1e-9766-e30eb5d7b5b3.png">

## The challenges
- Correctly reflecting what we learnt about cache coherence protocols from lecture in the actual implementation requires firm understanding of the protocol implications.
- Recoding traces from the program execution on multi-core machine and feeding those traces to our implementation is something none of us have experience before.
- Devising appropriate test plans, programs, and workloads in order to stress the simulator and extract valuable insights is also a challenge.
- Measuring performance of directory-based protocols depends highly on accurate modeling of inter-connect and arbitration.

## Resources
We'll start implementing the cache system from scratch. We plan to do development on local machines, and then gather traces, run tests and benchmarks on PSC machines. Another reason of using the PSC machine is because we want study the effect of number of cores on the scalability of different cache coherence implementations. We'll also use Intel Pin to record memory access traces on PSC machines.

## Goals and deliverables


