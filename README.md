# Rotating Mesh Simulation
This repository contains the files for the rotating mesh simulation using dynamic mesh properties and PIMPLE solver in openFOAM. PIMPle solver is know for solving the transient laminar and turbulent flow using Reynolds Averaged Navier Stokes Equations. This simulation was done on a simplified and custom propeller design to test the simulation setting for an average mesh to run faster and quicker on a heavy gaming laptop. 

https://user-images.githubusercontent.com/106860954/219719945-2f4b4060-fe8a-41bf-b598-7f07a9b01aae.mp4

<h1>Simulation details</h1>
<ul><h3>Openfoam Files</h3>
<li> 0 </li>
<li> Constant </li>
<li> System </li>
</ul>


<p align=justified> The 0 folder contains the variable files such as k , omega , nut , U and p. these file constain the information on the boundary and their condition at time step of 0 sec. Next in the constant folder where you can find the information on the mesh and the boundary faces which would be created under polymesh folder once you run the blockmesh command and the snappyHexmesh command. The trisurface folder contains the geometry of the propeller as well as the boundary in .STL format which could be easily used by the openFoam tools to read the geometry in asiic format. Last but not the least the system folder contains the simulation directory where the solver conditions are provided with the mesh directory as well. With the help of decomposepardict you can deconstruuct and reconstruct the mesh during the parallel processing and the cotrolDict consit of the simulation parameters such as the type of solver, time steps, deltaT and much more.These files could also be copeid from the OpenFOAM tutorials folder depending on the type of problem you are working on.</p>
 




