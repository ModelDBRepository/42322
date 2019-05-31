Directory:  /Examples/Accuracy/Luscher_Shiner

Source:  Luscher and Shiner (1990) Computation of action 
potential propagation and presynaptic bouton activation in 
terminal arborizations of different geometries.  Biophys. 
J.  58: 1377-1388.

Description:

The purposes of this model are: 1) to test the ability of 
SNNAP to reproduce aspects of a model developed by Luscher 
and Shiner (1990); and 2) demonstrate a method for modeling 
branching structures.  Only the first two figures in the 
paper were reproduced by this model.  Briefly, a parent 
axon gives rise to 7 or 9 daughter branches (Fig. 1 of 
Luscher and Shiner, 1990).  An action potential is able to 
propagating through the branch point with 7 daughter 
branches, but fails to propagate when the number of 
daughter branches is increased to 9.  Briefly, the 
properties of the model are homogenous and are described by 
a Hodgkin-Huxley model that has been adjusted to 22.5 C.  
Each process is described by 10 compartments and each 
compartment is the equivalent of 0.2 x the resting space 
constant.

Three simulations are included in this example: 

F1_7brch.smu simulates conduction through a branch point 
with 7 daughter branches (i.e., the equivalent of Luscher 
and Shiner Fig. 1Bc (1990).  The results of this simulation 
are illustrated in Luscher_Shiner_Fig_1Bc.jpg.

F1_9brch.smu simulates conduction block at a branch point 
with 9 daughter branches (i.e., the equivalent of Luscher 
and Shiner Fig. 1Bd (1990).  The results of this simulation 
are illustrated in Luscher_Shiner_Fig_1Bd.jpg.

F2.smu simulates the increase in the amplitude of a 
propagating spike as it approached a sealed end (i.e., the 
equivalent of Luscher and Shiner Fig. 2 (1990).  The 
results of this simulation are illustrated in 
Luscher_Shiner_Fig_2.jpg.

While developing a model of a branched structure, one must 
careful how to compute the cytoplasmic resistance at the 
branch point.  There are two methods.  The first is 
described by DeSchutter and Steuber (2001, Modeling simple 
and complex active neurons.  In: DeSchutter (Ed.) 
Computational Neuroscience, CRC Press, New York, pp. 233-
258).  The present simulation illustrates a second method.  
A 'dumby' compartment (brch.neu) is used to link the 
branches together.  The biophysical properties of the 
compartment are such that it doesn't significantly alter 
the properties of the model and the coupling conductances 
are adjusted as described by Parnas and Segev (1976, A 
mathematical model for conduction of action potentials 
along bifurcating axons.  J. Physiol. (Lond.), 295: 323-
343.
