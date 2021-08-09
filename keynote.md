---
layout: default
---

# Keynote talk

## Speaker:

![Thomas Fahringer](thomas.jpg)

Thomas Fahringer, Institute of Computer Science, University of Innsbruck, Austria

Thomas Fahringer is a Professor of Computer Science at the University of Innsbruck. He leads a research group in distributed and parallel processing, which develops the ASKALON system to support researchers worldwide in various fields of science and engineering to develop, analyze, optimize and run parallel and distributed scientific applications. Furthermore, he leads a research team that created the Insieme parallelizing and optimizing compiler for heterogeneous multicore parallel computers.
Fahringer was involved in numerous national and international research projects, including 15 EU-funded projects. He coordinated two H2020 projects, including AllScale - an exascale programming, multi-objective optimization, and resilience management environment based on nested recursive parallelism, 2015 - 2018, and the ENTICE project - Decentralized repositories for transparent and efficient virtual machine operations, 2015 - 2018. Fahringer has published 5 books, 40 journal and magazine articles, and more than 200 reviewed conference papers, including 4 best/distinguished IEEE/ACM papers.
email: tf@dps.uibk.ac.at

 
**On using modern C++ and nested recursive task parallelism for HPC applications with AllScale**


Contemporary parallel programming approaches often rely on well-established parallel libraries and language extensions to address specific HW resources, leading to mixed parallel programming paradigms. In contrast to these approaches, AllScale proposes a C++ template-based approach to ease developing scalable and efficient general-purpose parallel applications. Applications utilize a pool of parallel primitives and data structures for building solutions to their domain-specific problems. HPC experts who provision high-level, generic operators and data structures for common use cases design these parallel primitives. The supported set of constructs may range from ordinary parallel loops, over stencil and distributed graph operations, and frequently utilized data structures including (adaptive) multidimensional grids, trees, and irregular meshes, to combinations of data structures and operations like entire linear algebra libraries. This set of parallel primitives is implemented using pure C++ and may be freely extended by third-party developers, similar to conventional libraries in C++ development projects. One of the peculiarities of AllScale is its main source of parallelism based on nested recursive task parallelism. Sophisticated compiler analysis determines the data needed for every task, which is paramount to achieving performance across various parallel architectures. Experimental results for several applications implemented with AllScale will be shown.
