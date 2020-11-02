---
layout: wiki
title: Brillouin-Wigner Methods
categories: qm_further
---

#### 1. Wigner's 1935 paper: "on the modification of the Rayleigh-Schrödinger pertubation theory"
The Rayleigh-Schrödinger pertubation theory gives an explicit power series in $\lambda$ for the characteristic values $F_n$ and the charateristic function $\phi_n$ of a Hermitian operator $H+\lambda V$

$$
\begin{equation}
(H+\lambda V)\phi_n = F_n\phi_n
\end{equation}
$$

if the corresponding quantities $E_n$ and $\psi_n$ for the unperturbed operator $H$ are known

$$
\begin{equation}
H\psi_n = E_n\psi_n
\end{equation}
$$

If the so-called matrix elements of $V$ are denoted, as usual, by

$$
\begin{equation}
V_{nm} = (\psi_n,V\psi_m) = V_{mn}^*
\end{equation}
$$

the first terms in the aforementioned series read

$$
\begin{align}
F_n^{(2)} &=E_n + \lambda V_{nn} + \lambda^2\sum_{k\ne n} \frac{|V_{nk}|^2}{E_n-E_k}\\
\phi_n^{(1)} &= \psi_n +\lambda\sum_{k\ne n} \frac{V_{kn}}{E_n-E_k}\psi_k
\end{align}
$$

Generally only these first terms of the series are used in actual calculations, the higher order terms become increasingly complicated, Rayleigh-Schrödinger perturbation theory can be inapplicable because the series diverges in cases when the lowest energy value is finite.

#### 2. Brillouin-Wigner perturbation theory
Total Hamiltonian 

$$
\begin{equation}
H = H_0 + \lambda V
\end{equation}
$$

where

$$
\begin{align}
H_0\phi_k &= E_k\phi_k \\
H\psi_\mu &= \epsilon_\mu \psi_\mu \label{eq-qm-1}
\end{align}
$$

Eq.$\eqref{eq-qm-1}$ allows Schrödinger equation to be written in the form

$$
\begin{equation}
\big(\epsilon_\mu - H_0\big)\psi_\mu = \lambda V\psi_\mu
\end{equation}
$$

which can be rewritten  in matrix form

$$
\begin{equation}
\langle\phi_m|\psi_\mu\rangle = \frac{\lambda\langle\phi_m|V|\psi_\mu\rangle}{\epsilon_\mu-E_m}
\end{equation}
$$

It is convenient to put

$$
\begin{equation}
\langle \phi_\mu|\psi_\mu\rangle = 1
\end{equation}
$$

in order to simplify the formulae, thus, $\psi_\mu$ is not normalized to unity.

$$
\begin{align}
|\psi_\mu\rangle &= \sum_m |\phi_m\rangle\langle \phi_m|\psi_\mu\rangle \\
& = |\phi_\mu\rangle\langle\phi_\mu|\psi_\mu\rangle + \sum_{m\ne\mu}|\phi_m\rangle\langle\phi_m|\psi_\mu\rangle \\
& = |\phi_\mu\rangle + \lambda\sum_{m\ne\mu}|\phi_m\rangle\frac{1}{\epsilon_\mu-E_m}\langle\phi_m|V|\psi_\mu\rangle \label{eq-sbwpt}
\end{align}
$$

Eq.$\eqref{eq-sbwpt}$ is the basic formula of the Brillouin-Wigner perturbation theory for a single reference function, and from this we can develop a series expansion for the exact eigenfunction $\psi_\mu$, in power of $\lambda$ with coefficients depending on the perturbed energy $\epsilon_\mu$, rather than the energy of the model $E_m$, as would be the case in the more familiar Rayleigh-Schrödinger perturbation series.

Introducing the Brioullin-Wigner type propagator

$$
\begin{equation}
B = B(\mu) = \sum_{m\ne\mu}|\phi_m\rangle\frac{1}{\epsilon_\mu-E_m}\langle\phi_m|
\end{equation}
$$

then 

$$
\begin{align}
|\psi_\mu\rangle &= \big(1+\lambda BV + \lambda^2BVBV+\cdots\big)|\phi_\mu\rangle \\
\epsilon_\mu &=E_\mu + \lambda\langle \phi_\mu|V|\phi_\mu\rangle + \lambda^2\langle\phi_\mu| VBV|\phi_\mu\rangle +\cdots
\end{align}
$$

#### 3. Comparition of Rayleigh-Schrödinger and Brioullin-Wigner perturbation theories



#### 4. BWPT Further
> An important feature of modern perturbation theory is the so-called partitioning technique. In 
> this procedure, the functional space for the wave function is seperated into two parts, a model 
> space and an orthogonal space. The basic idea is to find "effective operators" which act only 
> within the limited model space but which generate the same result as do the original operators 
> acting on the entire functional space.


