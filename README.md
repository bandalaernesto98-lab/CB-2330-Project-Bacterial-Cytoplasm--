# CB-2330-Project-Bacterial-Cytoplasm--
Final project for the CB-2330 based on the scientific paper publishhd by Ido Golding and Edward C. Cox (2006).

On this project, we worked with a reference value for the ratio of the sub diffusive exponent of mRNA molecules observed on bacterial cytoplasm (ᵅ) and the power law used to describe the displacement behavior of the observed mRNA molecules.

With said reference value and formula we generated a stochastic model (using a Monte Carlo approach) to then calculate the mean squared displacement (MSD) values of 300 molecules of the mRNA at selected time lags (τ). By fitting the relationship MSD(τ) = Γ × τᵅ we estimated the generalized diffusion coefficient (Γ) and the sub diffusive exponential.

Once our model could correctly represent the expected diffusion behavior, we performed parameter sweeps for the cage time exponent (v) and the jump size parameter (σ), calibrating v by keeping the value that produced the most similar value of ᵅ as in the literature. We then investigated how varying σ affected Γ and compared those values with the established broad variability reported by Golding and Cox.

Paper's URL: https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.96.098102
