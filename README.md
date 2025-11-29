# CF-Flow Energies Dataset

This repository contains energies obtained using **CF-Flow**, a variational framework based on composite-fermion wavefunctions augmented with backflow transformations.

## Directory Structure

- **`gs_energies/`** — ground-state energies (total angular momentum **L = 0**)  
- **`tg_energies/`** —  Energies for states at filling ν = n / (p n + 1), corresponding to total angular momentum L = N / n + n − 1.

## File Naming Convention

Files follow the pattern:
N$(N)_nu$(num)_$(denom).txt


where:

- **N** — number of electrons  
- **nu = num/denom** — filling factor  

## File Contents

Each file contains rows corresponding to successive training checkpoints (earliest → latest).  
Columns:

1. **kappa** — Landau-level mixing strength  
2. **energy_per_particle** — density-corrected energy per particle  
3. **mcmc_error** — mcmc statistical uncertainty in the energy  
4. **local_energy_deviation** — average deviation of the local energy per particle (a diagnostic for how close the wavefunction is to an eigenstate/ground state)

## Citation

You are free to use and analyze these data.  
However, **any published results based on these files must cite**:

**Gattu *et al.* — _Dressing composite fermions with artificial intelligence_.**
