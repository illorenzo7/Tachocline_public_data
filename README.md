# Tachocline_public_data
To house many plots from low sigma tachocline simulations

To all Tachocline enthusiasts:

In this Github repository, I am in the process of compiling the main results of the global low-sigma tachocline models I’ve been running. I am starting with just two models to get us going (especially by tomorrow's COFFIES meeting, 11/15/2024). 

Recall some common features of these models:

- Solar like spherical shell with three critical radii: r_in, r_0, and r_out. r_0 is the transition between CZ and RZ.
- r_0/r_out = 0.759
- r_0 - r_in = r_out - r_0 (CZ is same width as RZ)
- It's a hydrostatic, perfect gas reference state with gamma = 5/3
- The background dS/dr switches from 0 in the CZ to an amplitude of O(1) in the RZ over transition region of width
- delta = 0.219
- g ~ 1/r^2
- Internal heating Q ~ rho * T in the CZ only
- nu, kappa, eta all ~ rho^(-1/2) (increase with height) 
- Stress free, impenetrable, fixed flux, potential field top and bottom boundaries
- "strict L conservation" is set to TRUE. This is really like another boundary condition. Should discuss at some point.
- There are three density scale heights across the CZ
- Cases are initialized from random small thermal (S) and magnetic (B) fields. All other fields start at 0.

- The cases all have the following SHARED nondimensional control parameters:
  Ra = 5.62 x 10^5 (fluxed-based Rayleigh number)
  Ro_c = 0.400 (convective Rossby number
  sigma = 0.3

- The cases only vary the Prandtl numbers:
  Pr and Pr_m.

- Note that
  N^2/(4\Omega_0^2) = sigma^2/Pr
  So low Pr means "stiffer" in this context. 
  
Some helpful conversions of timescales:
1 viscous diffusion time (VDT) = 149.5 x Pr^(-1/2) rotations
1 thermal diffusion time (TDT) = 149.5 x Pr^(+1/2) rotations
1 Eddington-Sweet time (EST) = 13.46 x Pr^(-1/2) rotations 

E.g., for Pr = 0.1:

1 VDT = 472.8 rotations
1 TDT = 47.3 rotations
1 EST = 42.6 rotations
