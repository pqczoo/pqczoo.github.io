---
layout: post
title:  "FrodoKEM on Embedded Devices"
date:   2018-07-25
categories: example post
---

Here is an example of what one might like to do with a _post_ after updating the table that relates to their research. A nice idea might be to simply copy and paste the abstract of the paper, point to any open source code of the research, or discuss any issues or open problems.

For example:

## Standard Lattice-Based Key Encapsulation on Embedded Devices
 by James Howe, Tobias Oder, Markus Krausz, and Tim Güneysu

**_Abstract_**: Lattice-based cryptography is one of the most promising candidates being
considered to replace current public-key systems in the era of quantum computing. In
2016, Bos et al. proposed the key exchange scheme FrodoCCS, that is also a submission
to the NIST post-quantum standardization process, modified as a key encapsulation
mechanism (FrodoKEM). The security of the scheme is based on standard lattices
and the learning with errors problem. Due to the large parameters, standard latticebased
schemes have long been considered impractical on embedded devices. The
FrodoKEM proposal actually comes with parameters that bring standard lattice-based
cryptography within reach of being feasible on constrained devices. In this work, we
take the final step of efficiently implementing the scheme on a low-cost FPGA and
microcontroller devices and thus making conservative post-quantum cryptography
practical on small devices. Our FPGA implementation of the decapsulation (the
computationally most expensive operation) needs 7,220 look-up tables (LUTs), 3,549
flip-flops (FFs), a single DSP, and only 16 block RAM modules. The maximum clock
frequency is 162 MHz and it takes 20.7 ms for the execution of the decapsulation. Our
microcontroller implementation has a 66% reduced peak stack usage in comparison
to the reference implementation and needs 266 ms for key pair generation, 284 ms for
encapsulation, and 286 ms for decapsulation. Our results contribute to the practical
evaluation of a post-quantum standardization candidate.

[https://eprint.iacr.org/2018/686.pdf](https://eprint.iacr.org/2018/686.pdf)


