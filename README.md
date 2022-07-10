# Central-and-Balanced-Configurations-with-a-small-mass
Numerical results of acentral and balanced configurations with an infinitesimal mass.

The files in the directories "BalancedConfig" and "CentralConfig" contain the
balanced and central configurations, respectively, computed by a stochastic 
optimization algorithm described in the paper (arXiv):
"A numerical analysis of planar central and balanced configurations in the 
(n+1)-body problem with a small mass" by Alexandru Doicu, Lei Zhao, and Adrian
Doicu. 

Central and balanced configurations in the (n+1)-body problem with a 
small mass are computed by means of 2 algorithms. 
 - The first algorithm relies on a direct solution method of the (n+1)-body 
   problem by using a stochastic optimization approach, while 
 - the second algorithm relies on an analytic-continuation method, which 
   involves as computational steps, the solutions of the n-body and the 
   restricted (n+1)-body problem, and the application of a local search 
   procedure to compute the final (n+1)-body configuration in the neighborhood 
   of the configuration obtained at the first two steps. 

The output file contains: 
1. Results related to the analytic-continuation method:
   - the number of solutions of the n-body problem NSOL(n), and for each kth
     solution of the n-body problem, the number of solutions of the restricted 
     (n+1)-body problem NSOL(k,n); 
   - the (total) number of solutions of the (n+1)-body problem NSOL(n+1) and 
     the number of distinct solutions excluding symmetries NSOL0(n+1);
   - for each configuration (K,L) of the (n+1)-body problem: (i) the Cartesian
     coordinates of the point masses (X,Y), (ii) the residual of the relative
     equilibrium equations FCT, and (iii) the RMS of the absolute error in
     Cartesian coordinates with respect to the initial guess; 
   - the residual of the normalization condition for the moment of inertia 
     FINERT and the Cartesian coordinates of the center of mass (XCM,YCM).      

2. Results related to the direct method:
   - the number of solutions of the (n+1)-body problem NSOL(n+1);
   - for each configuration of the (n+1)-body problem: (i) the Cartesian
     coordinates of the point masses (X,Y), (ii) the residual of the relative
     equilibrium equations FCT, and (iii) the RMS of the absolute error in 
     radial distances with respect to the analytic-continuation solution.

In the directory "BalancedConfig", the file "BCNMASxEXPMASy.dat" corresponds to a
a balanced configuration with x masses and mass parameter 10**(-y). Similarly, 
in the directory,"CentralConfig", the file "CCNMASxEXPMASy.dat" corresponds to a 
central configuration with x masses and mass parameter 10**(-y). 
