---
layout: post
title: Derivation of Lindblad Equation 
categories: quantum_mechanics
---
The Lindblad equation 
$$
\begin{align}
\frac{d\rho_S(t)}{dt} = \mathcal{L}\rho_S(t) = -i[H,\rho_S(t)] + \sum_i L_i\rho_S(t) L_i^\dagger -\frac{1}{2}\left\{L_i^\dagger L_i,\rho_S(t)\right\}，
\end{align}
$$
 > Some basic properties of open quantum system (maps) from defination

 $$
\begin{align}
\rho_S(t) = Tr_E\rho(t)=\mathcal{M}(\rho_S), \\
\end{align}
$$
where
$$ \rho(t)=U_{SE}\ \rho(0)\ U_{SE}^\dagger =U_{SE}\ (\rho_S\otimes \rho_E)\ U_{SE}^\dagger 
$$
therefore 
  1. Trace preservation: $Tr\rho_S(t)=Tr\rho_S(0)$
  2. Hermiticity preservation
  3. Positive: $\rho_S(t) \ge 0$
  4. It's complete positive (CP), meaning: $Id_A\otimes \mathcal{M}$ is positve over Hilbert space $\mathcal{H}_A\otimes\mathcal{H}_S$ for arbitrary $A$.

  > Remark: There are linear maps which are positive but not CP.
