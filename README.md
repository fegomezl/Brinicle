# On the simulation of a Brinicle

This repo contains the software used to simulate the formation of a brinicle, which is a hollow channel of ice that appears below the Artic sea surface, based on the model presented in the associated article.

## Abstract

Below the Arctic sea ice, under the right conditions, a flux of icy brine flows down into the sea. The icy brine has a much lower fusion point and is denser than normal seawater. As a result, it sinks while freezing everything around it, forming an ice channel called a brinicle (also known as ice stalactite). In this paper, we develop a mathematical model for this phenomenon, assuming cylindrical symmetry. The fluid is considered to be viscous and quasi-stationary. The heat and salt transport are weakly coupled to the fluid motion and are modeled with the corresponding conservation equations, accounting for diffusive and convective effects. Finite element discretization is employed to solve the coupled system of partial differential equations. We find that the model can capture the general behavior of the physical system and generate brinicle-like structures while also recovering dendrite composition, which is a physically expected feature aligned with previous experimental results. This represents the first complete model proposed that captures the global structure of the physical phenomenon even though it has some discrepancies, such as brine accumulation. 

## Citation

[![DOI](https://zenodo.org/badge/525176674.svg)](https://zenodo.org/badge/latestdoi/525176674)

```
@article{brinicle,
author = {Gómez-Lozada, Felipe  and del Valle, Carlos Andrés  and Jiménez-Paz, Julián David  and Lazarov, Boyan S.  and Galvis, Juan },
title = {Modelling and simulation of brinicle formation},
journal = {Royal Society Open Science},
volume = {10},
number = {10},
pages = {230268},
year = {2023},
doi = {10.1098/rsos.230268},
URL = {https://royalsocietypublishing.org/doi/abs/10.1098/rsos.230268},
eprint = {https://royalsocietypublishing.org/doi/pdf/10.1098/rsos.230268},
}
```

## Running the program

1. Copy the hidden file **.template\_local\_config.txt** with the name **local\_config.mk**
2. Add the MFEM instalation directory.
3. If you want to move the graphs to other folder after running a program, change the **NULL** option of the **SHARE\_DIR** variable to the folder directory.
4. If you want to chage some quantity on a simulation, in each folder the file **settings/parameters.mk** has all the main parameters of the simulation.
5. To run a simulation, you only have to write **make**.

## Results

Next some animations and images of the simulations are presented:

## Dendrites

<video src="https://user-images.githubusercontent.com/54986485/185271529-fdf337d3-3361-4ed0-8f1a-eac4cadc60a7.mp4" width="10%" height="10%">
</video> 

## Flow 100
<video src="https://user-images.githubusercontent.com/54986485/185271226-681fc74c-a7db-4b5e-9790-d1e7c4c1296a.mp4" width="10%" height="10%"> 
</video> 
 
## Flow 200
<video src="https://user-images.githubusercontent.com/54986485/185271415-f2edc37b-a756-4234-a726-ad0b8a82e7f9.mp4" width="10%" height="10%">
</video> 
  
## Flow 300
<video src="https://user-images.githubusercontent.com/54986485/185271429-3243bbc5-0ce5-4ef6-bdf6-2805222591be.mp4" width="10%" height="10%">
</video> 
   
## Flow 400
<video src="https://user-images.githubusercontent.com/54986485/185271475-5568f7e9-41b8-4845-baa0-a9e1fb274138.mp4" width="10%" height="10%">
</video> 

## Flow 500
<video src="https://user-images.githubusercontent.com/54986485/185271478-6495e560-097d-4d6d-b831-bd55e1cf0466.mp4" width="10%" height="10%">
</video> 
