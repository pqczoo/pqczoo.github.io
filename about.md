---
layout: page
title: About
permalink: /about/
order_number: 2
---

# About

This website was created in order to help with NIST's post-quantum standardisation process. A centralised website for these implementation results means they are much easier to find, and one can also discover what research has already been undertaken and what hasn't.

# How to add your own results

1. Head to the [GitHub repository](https://github.com/pqczoo/pqczoo.github.io/) of the website.
2. Find the data file of what table you wish to update:
  - The SCA table is found at [/_data/sca.yml](https://github.com/pqczoo/pqczoo.github.io/blob/master/_data/sca.yml).
  - The hardware table is found at [/_data/hardware.yml](https://github.com/pqczoo/pqczoo.github.io/blob/master/_data/hardware.yml). 
  - The microcontrollers table is found at [/_data/microcontrollers.yml](https://github.com/pqczoo/pqczoo.github.io/blob/master/_data/microcontrollers.yml).
3. Edit the file and add a new entry following the structure:
  - Hardware and microcontroller entries look like this:
    
    ```
    - Authors: James Howe, Tobias Oder, Markus Krausz, Tim Güneysu
      PQC Type: Lattice-Based
      Crypto Type: KEM
      Crypto Target: Frodo
      Device: Artix-7 FPGA
      Date: 17 July 2018
      Reference: eprint/2018/686
      Conference: CHES 2018
    ```
    
    - SCA entries similarly look like this:
    
    ```
    - Authors: Martin R. Albrecht and Amit Deo and Kenneth G. Paterson
      PQC Type: Lattice-Based
      Crypto Type: KEM
      Crypto Target: Kyber, NewHope
      Attack Type: Cold boot attack
      Date: 12 July 2018
      Reference: eprint/2018/672
      Conference: CHES 2018
    ```
    
4. Submit this change and then create a pull request. Once this has been approved the table will automatically update.
5. (Optional) Please add a new post about your addition! To do this just copy and paste the example file in the directory [_posts](https://github.com/pqczoo/pqczoo.github.io/tree/master/_posts), and rename the file to your choosing, but please ensure the file name begins with the date of the post. The example just includes the paper's abstract, but feel free to add more details if desired!
