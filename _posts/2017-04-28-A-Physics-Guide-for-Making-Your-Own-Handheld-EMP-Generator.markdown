---
layout: post
title:  "A Physics Guide for Making Your Own Handheld EMP Generator"
categories: EMP
tags: [emp]
---

A detailed walk-through of an EMP generator & an explanatory touch on the Maxwell's Equations.

When did you first hear about the term "EMP"? Maybe in some science fiction books, it may be described as some cannon-like weapons that shoot out some powerful light beams so any electronic device standing in the way is burned down with sparks in just a blink of an eye. Well, this is just the most imaginative part of the EMP. If you are interested to learn more, this blog will present the physics behind such device with a detailed guide for you to make your own EMP generator that only works against small electronic gadgets (for educational purposes).

## EMP Definition & Basics
EMP stands for electromagnetive pulse, which is a burst of eletromagnetic energy in a short time. To undnerstand what does the phrase "a burst of electromagnetic energy" actually mean, one need to learn about the concepts of electric field & potential, as well as the relationship between the electric & magnetic fields. First, the electric field & potential due to a point charge \\( Q_{source} \\) are shown below.

$$ \begin{equation} \vec{E} = k\frac{Q_{source}}{r^2} \hat{r} \end{equation} $$

$$ \begin{equation} V = -k\frac{Q_{source}}{r} \end{equation} $$

where \\( k \\) is known as the Coulomb's constant. 

Note that any charge particle \\( q \\) trapped inside an electric field experiences a force (eqn-3), and the electric field is defined as the negative spatial derivative of the electric potential (eqn-4). 

$$ \begin{equation} \vec{F}=\vec{E}q \end{equation} $$

$$ \begin{equation} \vec{E}=-\frac{dV}{d\vec{r}} \end{equation} $$

Second, according to the Maxwell's equations shown below, the 3rd equation -- Faraday's law of induction describes how a time-varying magnetic field induces an electric field, and the 4th equation -- Ampère's law with Maxwell's addition states that the magnetic field could be generated in two ways: either by moving charges (electric current) or by a changing electric field. 

| ![Maxwell.png](/assets/images/Maxwell.png) | 
|:--:| 
| *Maxwell's Equations describing electromagnetism.* |

Thus, EMP could be understood as either a mixture (i.e. electromagnetic radiation) or just the electric/magnetic energy (just a burst in electric or magnetic field, i.e. electric/magnetic pulse) that could cause/create a large change of the electric/magnetic fields surrounding the targeted electronics in a short time. If the EMP has enough energy to cause a large enough sudden change of the electric/magnetic field, it generally could cause excessive currents, short-circuits or reset the electronics components. In other words, the goal is to provide excessive energies to the charge carriers (i.e. electrons) so that they won't behave in the desired way. Depending on how strong the "burst of electromagnetic energy" is, EMP could cause malfunctions or destroy the electronic devices.

## EMP Design
One important thing we have learned in the previous section is that in order to generate an electrogmanetic pulse (EMP), we need to create “a burst of electromagnetic energy”, which is equivalent to a large, sudden change of either a magnetic or an electric field.

Indeed, it doesn't matter if we choose to create a electric or a magnetic pulse, because according to Maxwell's equations, a pulse of electric energy unavoidably generates a magnetic field, and leads to a pulse of magnetic energy. Generally, either the electric or the magnetic form of EMP will dominate.

Since it could be pretty dangerous to create a large pulse of electric field that could influence a typical electronic gadget, the design mainly involves the use of a coil to create a pulse of magnetic field (as the dominant form of EMP). There are two slightly different circuits to implement this kind of EMP generator with a small difference in terms of the power & performance of the EMP, which are presented below.

| ![Circuit1.png](/assets/images/Circuit1.png) | 
|:--:| 
| *EMP circuit design that utilizes a high-voltage generator to create electric arcs (also known as dielectric breakdown).* |

The principle behind the first design is to utilize the large, pulse-like current generated during the dielectric break down, which further creates a pulse-like magnetic field through the coil according to Ampère's law. Small high-voltage generators that convert a DC volage source of 6-12 V to 1000 kV are suitable for our purpose, and they are usually cheap to buy on Amazon or Ebay.

| ![Circuit2.png](/assets/images/Circuit2.png) | 
|:--:| 
| *EMP circuit design that utilizes a high-voltage generator to create electric arcs (also known as dielectric breakdown).* |

Similar to the first design, this second design utilize a photoflash capacitor that discharges all its stored electric energy in a very short time to generate a large pulse of current through the coil, leading to a single pulse of magnetic field. An example tutorial of this kind of EMP design could be found at [Wikihow](https://www.wikihow.com/Build-an-EMP-Generator).


The main difference between the two EMP designs above is that the first design creates a constant supply of irregular magnetic pulses with a relatively stable power, while the second design generates a large, powerful magnetic pulse and needs to be recharged before the next shot.

There are different ways to make your EMP stronger, and the drawing below shows 3 feasible options as suggested by the Maxwell's equations. Try come out more methods by first understanding the Maxwell's equations and see if you could make your EMP stronger!

| ![StrongerEMP.png](/assets/images/StrongerEMP.png) | 
|:--:| 
| *3 ways to make your EMP stronger!* |

Overal, I made my own EMP generator based on the first design, and below you will see some cool demonstration videos :)

| ![EMPdevice.png](/assets/images/EMPdevice.png) | 
|:--:| 
| *My simple EMP generator* |


## EMP showcase
I test the performance of my EMP generator with 3 electronic gadgets: TI-84 calculator, a small radio and an iPhone 5 SE. Thanks to the modern technology, most electronic devices today are either well-shielded or have a protective circuitry that prevents the device from being damaged by EMP (to a certain extent). For example, some devices shut down completely when being attacked by an EMP (i.e. TI-84) and requries a battery-removed reboot to work again. Cheaper electronic devices like the radio could be pretty vulnerable to EMP, as I eventually killed its FM option. The EMP I made seems to be too weak to disable the iPhone 5 SE -- all it can do is to mess up the LCD display.

| [![EMP vs TI-84](https://img.youtube.com/vi/j-VMMReCcNo/0.jpg)](https://youtu.be/j-VMMReCcNo) |
|:--:| 
| *EMP vs. TI-84* |

| [![EMP vs Radio](https://img.youtube.com/vi/PW5Wf-DimXE/0.jpg)](https://youtu.be/PW5Wf-DimXE) |
|:--:| 
| *EMP vs. Radio* |

| [![EMP vs iPhone 5](https://img.youtube.com/vi/KbRZXIsOMeg/0.jpg)](https://youtu.be/KbRZXIsOMeg) |
|:--:| 
| *EMP vs. iPhone 5 SE* |