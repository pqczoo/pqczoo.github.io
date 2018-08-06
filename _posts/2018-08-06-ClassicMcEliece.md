---
layout: post
title:  "Classic McEliece"
date:   2018-08-06
categories: hadware design
---

# FPGA-based Niederreiter Cryptosystem using Binary Goppa Codes
 by Wen Wang, Jakub Szefer, and Ruben Niederhagen

**_Abstract_**: This paper presents an FPGA implementation of the Niederreiter
cryptosystem using binary Goppa codes, including modules for encryption, decryption,
and key generation. We improve over previous implementations in terms of efficiency
(time-area product and raw performance) and security level. Our implementation is
constant time in order to protect against timing side-channel analysis. The design
is fully parameterized, using code-generation scripts, in order to support a wide
ange of parameter choices for security, including binary field size, the degree of
the Goppa polynomial, and the code length. The parameterized design allows us to
choose design parameters for time-area trade-offs in order to support a wide variety
of applications ranging from smart cards to server accelerators. For parameters that
are considered to provide "128-bit post-quantum security", our time-optimized
implementation requires 966,400 cycles for the generation of both public and private
portions of a key and 14,291 cycles to decrypt a ciphertext. The time-optimized design
uses only 121,806 ALMs (52% of the available logic) and 961 RAM blocks (38% of the
available memory), and results in a design that runs at about 250MHz on a medium-size
Stratix V FPGA.

[https://eprint.iacr.org/2017/1180.pdf](https://eprint.iacr.org/2017/1180.pdf)
