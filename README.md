# On the simulation of a Brinicle

This repo contains the software used to simulate the formation of a brinicle, which is a hollow channel of ice that appears below the Artic sea surface, based on the model presented in the associated article.

## Abstract

Below the Arctic sea ice, under the right conditions, a flux of icy brine flows down into the sea. The icy brine has a much lower fusion point and is denser than normal seawater. As a result, it sinks while freezing everything around it, forming an ice channel called a brinicle (also known as ice stalactite). We simulate this phenomenon assuming cylindrical symmetry. The fluid is considered viscous and quasi-stationary, and the problem is formulated by taking advantage of the setup symmetries. The heat and salt transport are weakly coupled to the fluid motion and are modeled with the corresponding conservation equations, accounting for the diffusive and convective effects. The coupled system of partial differential equations is discretized and solved with the help of the MFEM finite element library. With the simulation, we were able to capture the general behavior of a system undergoing a phase change. Although there are some discrepancies with the physical system such as brine accumulation, we managed to generate brinicle-like structures with the model proposed using low temperatures and flows while also recovering dendrite composition, which is a physically expected feature from the system. 

## Citation

```
@article{brinicle,
  title = {On the simulation of a Brinicle},
  author = {Felipe G\'{o}mez and Carlos Andr\'{e}s del Valle and Jili\'{a}n Jim\'{e}nez},
  journal = {},
  doi = {},
  volume = {},
  pages = {},
  year = {2022}
}
```

## Running the program

1. Copy the hidden file **.template\_local\_config.txt** with the name **local\_config.mk**
2. Add the MFEM instalation directory.
3. If you want to move the graphs to other folder after running a program, change the **NULL** option of the **SHARE\_DIR** variable to the folder directory.
4. If you want to chage some quantity on a simulation, in each folder the file **settings/parameters.mk** has all the main parameters of the simulation.
5. To run a simulation, you only have to write **make**.

## Results

Next some runs for the simulation are presented.

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
