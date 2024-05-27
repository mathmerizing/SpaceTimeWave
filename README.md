# Space-Time Finite Element Method for wave equation
Solving the wave equation as a first-order system in time using space-time finite elements.

## Problem statement
The strong form of the wave equation is given by

$$
\partial_{tt} u - \partial_{xx} u = f \qquad \forall x \in \Omega, t \in [0,T].
$$

As a firs-order system in time this reads

$$
\partial_t v - \partial_{xx} u = f,
$$

$$
\partial_t u = v.
$$

Usually the wave equation is complemented with the initial conditions for $u$ and $v$ which are given as

$$
u(x, 0) = u^0(x),
$$

$$
v(x, 0) = v^0(x).
$$

However, in a recent publication on space-time variatonal material modeling Junker and Wick [[1]](#1) derived that instead one should have an initial and a final condition for the velocity $v$, i.e.



## Running the code locally 
Install FEniCS, NumPy and matplotlib.
Running the normal wave equation:
```
jupyter notebook Wave_Normal.ipynb
```

Running the wave equation with initial and final condition for velocity:
```
jupyter notebook Wave_FinalCondition.ipynb
```

## Running the code on Google Colab
Link for the normal wave equation: 

https://githubtocolab.com/mathmerizing/SpaceTimeWave/blob/main/Wave_Normal.ipynb

Link for the wave equation with initial and final condition for velocity: 

https://githubtocolab.com/mathmerizing/SpaceTimeWave/blob/main/Wave_FinalCondition.ipynb

## References
<a id="1">[1]</a>
Junker, P., Wick, T. Space-time variational material modeling: a new paradigm demonstrated for thermo-mechanically coupled wave propagation, visco-elasticity, elasto-plasticity with hardening, and gradient-enhanced damage. Comput Mech 73, 365–402 (2024). https://doi.org/10.1007/s00466-023-02371-2
