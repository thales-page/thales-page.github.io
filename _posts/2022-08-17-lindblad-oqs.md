---
layout: post
title: Derivation of Lindblad Equation 
categories: quantum_mechanics
---
The Lindblad equation 
$$
\begin{align}
\frac{d\rho_S(t)}{dt} = \mathcal{L}\rho_S(t) = -i[H,\rho_S(t)] + \sum_i L_i\rho_S(t) L_i^\dagger -\frac{1}{2}\left\{L_i^\dagger L_i,\rho_S(t)\right\}
\end{align}
$$
 > some basic properties of open quantum system (maps) from defination
 $$
\begin{align}
\rho_S(t) = \text{Tr}_E\rho(t), \quad \rho(t)=U_{SE}\ \rho(0)\ U_{SE}^\dagger =U_{SE}\ (\rho_S\otimes \rho_E)\ U_{SE}^\dagger
\end{align}
 $$
  - Trace preservation 
  -  Hermiticity preservation
  - Positive
