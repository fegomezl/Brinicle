# On the simulation of a Brinicle

Below the Arctic sea ice, under the right conditions, a flux of icy brine flows down into the sea. The icy brine has a much lower fusion point and a higher density than normal seawater. As a result, it sinks while freezing everything around it, forming an ice channel called a brinicle (also known as ice stalactite). We simulate this phenomenon assuming cylindrical symmetry. The fluid is considered viscous and quasi-stationary, and the problem is simulated, taking advantage of the setup symmetries. The heat and salt transport are weakly coupled to the fluid motion and are modeled with the corresponding conservation equations, taking into account diffusive and convective effects. The coupled system of partial differential equations is discretized and solved with the help of the MFEM finite element library. 

## Citation

```
@article{mfem,
 title = {On the simulation of a Brinicle},
 author = {Felipe Gómez and Carlos Andrés del Valle and Jilián Jiménez},
 journal = {},
 doi = {},
 volume = {},
 pages = {},
 year = {2022}
}
```

## Results

## Flow 100
<video src="https://user-images.githubusercontent.com/54986485/184774459-eaa6ea77-1bbd-4c0e-8a4d-8c6332b5000f.mp4" width="50%" height="50%"> 
</video> 
 
## Flow 200
<video src="https://user-images.githubusercontent.com/54986485/184775336-29bc8db5-5b58-4976-ac1b-e2dfe193cee3.mp4" height="5">
</video> 
  
## Flow 300
<video src="https://user-images.githubusercontent.com/54986485/184775367-ff9b1c6d-c6a6-42a4-b3c8-f70586b1b518.mp4" height="5">
</video> 
   
## Flow 400
<video src="https://user-images.githubusercontent.com/54986485/184775387-65937ad2-91b5-48a3-a351-0d6d7a6fc93f.mp4" height="5">
</video> 
    
## Flow 500
<video src="https://user-images.githubusercontent.com/54986485/184775404-b8c629d3-66bd-42e2-a2fe-ae02a82753d2.mp4" height="5">
</video> 


## Running the programs

1. Copy the hidden file **.template\_local\_config.txt** with the name **local\_config.mk**
2. Add the MFEM instalation directory.
3. If you want to move the graphs to other folder after running a program, change the **NULL** option of the **SHARE\_DIR** variable to the folder directory.
4. If you want to chage some quantity on a simulation, in each folder the file **settings/parameters.mk** has all the main parameters of the simulation.
5. To run a simulation, you only have to write **make**.
