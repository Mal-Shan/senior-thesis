# Senior Thesis Code 

- When creating the code for this simulation, two classes of conditions were considered:
  - The first class (which comprises simulations 1-3) assumes that there is no hierarchical structure present within the simulated data (such that each i scan is from a different patient).
  - The second type assumes that there is a hierarchical structure present within the simulated data (simulations 4 - 9), such that every pair of scans is from the same patient.
 
- Within the second type of conditions, data was simulated assuming that either every pair of scans had different covariate values (simulations 5-8) or the same covariate values (simulations 9-12) for x1 and x2.
  
- For every group of three conditions, various parameters were modified to test the model correction’s performance, specifically: a) a tuned beta_0 parameter, b) the correlation between covariates (as defined in their multivariate normal distribution), and c) the effect of the confounding covariate (diabetes duration) on the outcome variable (through modifications of 𝛽2).
  
- It is important to note that the tuned beta_0 parameter was derived by ensuring that the probability function used to generate the y outcomes was as close to the original p_0 from the dataset. 
