---
layout: default
---

# Accpeted papers


## Accelerating Messages by Avoiding Copies in an Asynchronous Task-based Programming Model

*Authors:* Nitin Bhat, Sam White, and Laxmikant V Kale

Communication is critical to the scalable and efficient performance of scientific simulations on extreme-scale computing systems. Part of the promise of task-based programming models is that they can naturally overlap communication with computation and exploit locality between tasks. Copy-based semantics using eager communication protocols easily enable such asynchrony by alleviating the responsibility of buffer management from the user, both on the sender and the receiver. However, these semantics increase memory allocations and copies and in turn, affect application memory footprint and performance, especially with large messages.
In this work, we extend the Charm++ programming model with so-called "zero copy" messaging semantics. These semantics work on user-provided buffers and do not semantically require copies by either the user or the runtime system. This enables in-place data movement of various kinds. We motivate our work by reviewing the existing messaging models supported by Charm++, identify their semantic shortcomings with respect to large message handling, and define new APIs for communication based on RDMA capabilities. We demonstrate the utility of our new communication interfaces by the use of benchmarks written in Charm++ and AMPI. The result is up to 90% of message latency improvement and nearly 2x lower peak memory usage.

## Combining OpenMP tasking and target (GPU) offloading for productivity and performance on heterogeneous systems

*Authors:* Pedro Valero-Lara, Jungwon Kim, Oscar Hernandez, and Jeffrey Vetter

We evaluate the use of OpenMP tasking with target (GPU) offloading as a potential solution for programming productivity and performance on heterogeneous systems. As test case, We use one of the most popular and widely used BLAS Level-3 routines, triangular solver(TRSM). To benefit from the heterogeneity of the current HPC systems, we propose a different parallelization of the algorithm by using a non-uniform decomposition of the problem. We use target (GPU) offloading inside OpenMP tasks to deal with the heterogeneity found in the hardware. This new approach is able to outperform the state-of-the-art algorithms, which use a uniform decomposition of the data, on both: CPU only and CPU+GPU systems, reaching speedups of up to one order of magnitude. The performance achieved by this approach is faster than the IBM ESSL math library on CPU and competitive w.r.t. a highly optimized heterogeneous CUDA version. For the performance analysis, we have used one node of the ORNL's supercomputer Summit.

## FleCSI 2.0: The Flexible Computational Science Infrastructure Project

*Authors:* Ben Bergen, Irina Demeshko, Charles Ferenbaugh, Davis Herring, Li-Ta Lo, Julien Loiseau, Navamita Ray and Andrew Reisner

The FleCSI 2.0 programming system supports multiphysics application development through a runtime abstraction layer, and by providing core topology types that can be customized for speciﬁc numerical methods. The abstraction layer provides a single-source programming interface for distributed and shared-memory data parallelism through task and kernel execution, and has been demonstrated to introduce virtually no runtime overhead. FleCSI's core topology types represent a rich set of basic data structures that can be specialized to create application-facing interfaces for a variety of diﬀerent physics packages. Using the FleCSI control and data models, it is straightforward to compose multiple packages to create full multiphysics applications. When used with the Legion backend, FleCSI oﬀers extended runtime analysis that can increase task concurrency, facilitate load balancing, and allow for portability across heterogeneous computing architectures.

## An Experimental Study of SYCL Task Graph Parallelism for Large-Scale Machine Learning Workloads

*Authors:* Cheng-Hsiang Chiu, Dian-Lun Lin, and Tsung-Wei Huang

Task graph parallelism has emerged as an important tool to efficiently execute large machine learning workloads on GPUs. Users describe a GPU workload in a task dependency graph rather than aggregated GPU operations and dependencies, allowing the runtime to run whole-graph scheduling optimization to significantly improve the performance. While the new CUDA graph execution model has demonstrated significant success on this front, the counterpart for SYCL, a general-purpose heterogeneous programming model using standard C++, remains nascent. Unlike CUDA graph, SYCL runtime leverages out-of-order queues to implicitly create a task execution graph induced by data dependencies. For explicit task dependencies, users are responsible for creating SYCL events and synchronizing them at a non-negligible cost. Furthermore, there is no specialized graph execution model that allows users to offload a task graph directly onto a SYCL device in a similar way to CUDA graph. This paper conducts an experimental study of SYCL's default task graph parallelism by comparing it with CUDA graph on large-scale machine learning workloads in the recent HPEC Graph Challenge. Our result highlights the need for a new SYCL graph
execution model in the standard.

## Understanding the Effect of Task Granularity on Execution Time in Asynchronous Many-Task Runtime Systems

*Authors:* Shahrzad Shirzad, Rod Tohid, Alireza Kheirkhahan, Bibek Wagle and Hartmut Kaiser

Task granularity is a key factor in determining the performance of asynchronous many-task (AMT) runtime systems. The over-head of scheduling an excessive number of tasks with smaller granularities causes performance degradation while creating a few larger tasks leads to starvation and therefore under-utilization of resources. In this paper, we developed an analytical model of the execution time of an application with balanced parallel for-loops in terms of grain size, and number of cores. The parameters of this model mostly depend on the runtime and the architecture. We introduce an approach to suggest a range of possible grain sizes to achieve the best performance based on the proposed model. To the best of our knowledge, our analytical model is the first to explain the relationship between the execution time in terms of grain size, runtime, and physical characteristics of the machine in an asynchronous runtime system.
