---
layout: post
title:  "A Compact and Scalable Hardware/Software Co-design of SIKE"
date:   2020-06-25
categories: hardware design
---

## A Compact and Scalable Hardware/Software Co-design of SIKE
 by Pedro Maat C. Massolino and Patrick Longa and Joost Renes and Lejla Batina

**_Abstract_**: We present efficient and compact hardware/software co-design 
implementations of the Supersingular Isogeny Key Encapsulation (SIKE) protocol 
on field-programmable gate arrays (FPGAs). In order to be better equipped for 
different post-quantum scenarios, our architectures were designed to feature 
high-flexibility by covering all the currently available parameter sets and 
with support for primes up to 1008 bits. In particular, any of the current SIKE 
parameters equivalent to the post-quantum security of AES-128/192/256 and SHA3-256 
can be selected and run on-the-fly. This security scalability property, 
together with the small footprint and efficiency of our architectures, makes 
them ideal for embedded applications in a post-quantum world. 
In addition, the proposed implementations exhibit regular, constant-time execution, 
which provides protection against timing and simple side-channel attacks. 
Our results demonstrate that supersingular isogeny-based primitives such as SIDH and SIKE 
can indeed be deployed for embedded applications featuring competitive performance. 
For example, our smallest architecture based on a 128-bit MAC unit takes only 3855 slices, 
21 BRAMs and 57 DSPs on a Virtex 7 690T and can perform key generation, encapsulation and 
decapsulation in 14.2, 24.1 and 25.7 milliseconds for SIKEp434 
and in 51.7, 85.4 and 92.1 milliseconds for SIKEp751, respectively. 

[https://eprint.iacr.org/2020/040.pdf](https://eprint.iacr.org/2020/040.pdf)
[https://github.com/pmassolino/hw-sike](https://github.com/pmassolino/hw-sike)


