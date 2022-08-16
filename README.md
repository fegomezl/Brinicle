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

![til](https://github.com/fegomezl/Brinicle/tree/main/animations/100.mp4)

![til](https://github.com/fegomezl/Brinicle/tree/main/animations/200.mp4)

![til](https://github.com/fegomezl/Brinicle/tree/main/animations/300.mp4)

![til](https://github.com/fegomezl/Brinicle/tree/main/animations/400.mp4)

![til](https://github.com/fegomezl/Brinicle/tree/main/animations/500.mp4)

## Running the programs

1. Copy the hidden file **.template\_local\_config.txt** with the name **local\_config.mk**
2. Add the MFEM instalation directory.
3. If you want to move the graphs to other folder after running a program, change the **NULL** option of the **SHARE\_DIR** variable to the folder directory.
4. If you want to chage some quantity on a simulation, in each folder the file **settings/parameters.txt** has all the main parameters of the simulation.
5. To run a simulation, you only have to write **make**.
