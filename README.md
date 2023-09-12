# SimulationSetting
This file contains the simulation setting in abstract submitted to BAYSM 2023 

# Simulation Setting 
X pretreatment covariates: X1 ~ N(1, 1); X2 ~ Pois(2); X3 ~ Unif(-1, 1)

A treatment assignment: A~Bernouli(0.5)

Y outcome: Y = X1 + X2 + X3 + A + AX1 - AX2 + epsilon

epsilon ~ N(0, 2)

The selection mechanism 

p = F(-5.087 + X1 + X2 + X3) where F(.) is the cumulative distribution function of the logistic distribution.

S ~ Bernouli(p)

The total sample n was set at 500, 1000, 2000, and 5000 to generate 1000 simulated datasets respectively.

# Hypothetical Scenario
Under the same simulation setting with n = 1000, we generated one simulated dataset with 193 selected patients, The average treatment effect for
s
the observed sample is -0.635 and the pooled sample variance is 7.2.

To attain 85% power at a 5% significance level for the one-sided test, the future trial is designed with a sample size of 258 patients based on the observed samples.

The PPoS is calculated as the average power across the posterior distribution of ATE under this design.
