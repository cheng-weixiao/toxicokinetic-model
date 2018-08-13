# toxicokinetic-model

Diffusion-Limited PBPK for PFOA in Male Rats, see [the paper](https://pubs.acs.org/doi/abs/10.1021/acs.est.7b02602) published on Environmental Science & Technology


The purpose of this model is to predict the toxicokinetics and tissue
distributioin of PFOA in male rats without the need to fit experimental
data.

This version implements Monte Carlo uncertainty analysis. Parameter
values are therefore chosen from distributions (normal, lognormal,
or uniform, see [Supporting Information](https://pubs.acs.org/doi/suppl/10.1021/acs.est.7b02602) Section S4 for details) over 10,000 iterations.

The code below is parameterized to replicate the conditions of the 1 mg/kg
IV dose experiment from the Kemper (2003) study.
For the code for other dose experiments, the paramters including body
weight(BW), Dose, and sampling time (seconds) need to be modified to
corresponding values based on different studies. Moreover, the initial
condition is different between IV and oral dose treatment.
