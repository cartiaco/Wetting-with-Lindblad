# Wetting-with-Lindblad

In this repository, we provide the numerical codes used in the article *Wetting critical behavior within the Lindblad dissipative dynamics* by C. Artiaco, A. Nava, and M. Fabrizio (Ref.[1](https://arxiv.org/abs/2206.11662)) to study the critical behavior, both in space and time, of the wetting interface within the coexistence region around the first-order phase transition of a fully-connected quantum Ising model in a slab geometry. For that, we employ a simple Lindblad master equation in which temperature is inherited by the coupling to a dissipative bath rather than being a functional parameter as in the conventional Cahn’s free energy. 

## Description

In Ref.1, we show that the wetting critical behavior in our model can be studied by solving a set of coupled first-order, non-linear differential equations (see Eqs.(23) and (26) in Ref.1). We refer to Ref.1 for any further detail about the model, baths, derivation of the set of differential equations giving the wetting dissipative dynamics, and results. 

Here, we provide the [Mathematica notebook](https://github.com/cartiaco/wetting-with-Lindblad/blob/main/multi-layer-system.nb) solving the set of differential equations for the magnetization of the slab's layers, valid for any value of the Hamiltonian parameters (in particular, the transverse magnetic field $h_x$, see Eq.(2) in Ref.1), and temperature $T$. The notebook provides also some example plots of the results, as the ones reported [here](https://github.com/cartiaco/Wetting-with-Lindblad/edit/main/Figures). 

## Details on the numerical implementation

To make the code more efficient, we solve explicitly a differential equation for each component of the magnetization for each layer in the bulk. The explicit equations can be found easily from the definitions of $\mathbf{v}^3(t), \mathbf{v}^+(t), \mathbf{v}^-(t)$ (see Eqs.(19)-(23)). 

Please notice that in our setup the states of the first and last layer are fixed in the ordered and disordered state, respectively (i.e., they do not evolve in time). 

## Code

The notebook is fully written in the [Wolfram Language](https://www.wolfram.com/language/) and can be used via the [Wolfram Mathematica](https://www.wolfram.com/mathematica/) software system.

## References

The codes in this repository are freely available; please acknowledge their use by referring to:

1. C. Artiaco, A. Nava, M. Fabrizio, Wetting critical behavior within the Lindblad dissipative dynamics, [arXiv2206.11662](https://arxiv.org/abs/2206.11662)
