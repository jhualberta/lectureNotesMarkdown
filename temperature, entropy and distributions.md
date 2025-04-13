References: 

[Negative temperature - Wikipedia](https://en.wikipedia.org/wiki/Negative_temperature)
[Rényi entropy - Wikipedia](https://en.wikipedia.org/wiki/R%C3%A9nyi_entropy)
[Tsallis entropy - Wikipedia](https://en.wikipedia.org/wiki/Tsallis_entropy)
John C. Baez. What is Entropy?

------
## Noninteracting two-level particles

For a system with N particles, each of which can take an energy of either $+\epsilon$ or $-\epsilon$ but are otherwise noninteracting. The total energy of the system is
$$E = \epsilon \sum_{i=1}^N\sigma_i = \epsilon_j$$

for the $i$-th particle, $\sigma_i$ = 1 or -1. Assume that $j$ positive particles remain after canceling out the $+\epsilon$ and $-\epsilon$ particles.



E=ε∑i=1Nσi=εj![{\displaystyle E=\varepsilon \sum _{i=1}^{N}\sigma _{i}=\varepsilon j}](https://wikimedia.org/api/rest_v1/media/math/render/svg/1ff69a9190667f1602e9a168d11df452497fa498)

where σi is the sign of the ith particle and j is the number of particles with positive energy minus the number of particles with [negative energy](https://en.wikipedia.org/wiki/Negative_energy "Negative energy"). From elementary [combinatorics](https://en.wikipedia.org/wiki/Combinatorics "Combinatorics"), the total number of [microstates](https://en.wikipedia.org/wiki/Microstate_(statistical_mechanics) "Microstate (statistical mechanics)") with this amount of energy is a [binomial coefficient](https://en.wikipedia.org/wiki/Binomial_coefficient "Binomial coefficient"):

ΩE=(NN+j2)=N!(N+j2)!(N−j2)!.![{\displaystyle \Omega _{E}={\binom {N}{\frac {N+j}{2}}}={\frac {N!}{\left({\frac {N+j}{2}}\right)!\left({\frac {N-j}{2}}\right)!}}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/18eaf5837a50269e351dc365eed4cc889dd25225)

By the [fundamental assumption of statistical mechanics](https://en.wikipedia.org/wiki/Fundamental_assumption_of_statistical_mechanics "Fundamental assumption of statistical mechanics"), the entropy of this [microcanonical ensemble](https://en.wikipedia.org/wiki/Microcanonical_ensemble "Microcanonical ensemble") is

S=kBln⁡ΩE![{\displaystyle S=k_{\text{B}}\ln \Omega _{E}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/7bab5d076397a78a3f830de7d1a6ab1d4324f1ce)

We can solve for thermodynamic beta (_β_ = ⁠1/_k_B_T_⁠) by considering it as a [central difference](https://en.wikipedia.org/wiki/Central_difference "Central difference") without taking the [continuum limit](https://en.wikipedia.org/wiki/Continuum_limit "Continuum limit"):

β=1kBδ2ε[S]2ε=12ε(ln⁡ΩE+ε−ln⁡ΩE−ε)=12εln⁡((N+j−12)!(N−j+12)!(N+j+12)!(N−j−12)!)=12εln⁡(N−j+1N+j+1).![{\displaystyle {\begin{aligned}\beta &={\frac {1}{k_{\mathrm {B} }}}{\frac {\delta _{2\varepsilon }[S]}{2\varepsilon }}\\[3pt]&={\frac {1}{2\varepsilon }}\left(\ln \Omega _{E+\varepsilon }-\ln \Omega _{E-\varepsilon }\right)\\[3pt]&={\frac {1}{2\varepsilon }}\ln \left({\frac {\left({\frac {N+j-1}{2}}\right)!\left({\frac {N-j+1}{2}}\right)!}{\left({\frac {N+j+1}{2}}\right)!\left({\frac {N-j-1}{2}}\right)!}}\right)\\[3pt]&={\frac {1}{2\varepsilon }}\ln \left({\frac {N-j+1}{N+j+1}}\right).\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/db0815c0bf86f998d695c49c64d19a469413e027)

hence the temperature

T(E)=2εkB[ln⁡((N+1)ε−E(N+1)ε+E)]−1.![{\displaystyle T(E)={\frac {2\varepsilon }{k_{\text{B}}}}\left[\ln \left({\frac {(N+1)\varepsilon -E}{(N+1)\varepsilon +E}}\right)\right]^{-1}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/3b08f5b054948d53bea8127d95134a27e613b39e)

This entire proof assumes the microcanonical ensemble with energy fixed and temperature being the emergent property. In the [canonical ensemble](https://en.wikipedia.org/wiki/Canonical_ensemble "Canonical ensemble"), the temperature is fixed and energy is the emergent property. This leads to (ε refers to microstates):

Z(T)=∑i=1Ne−εiβE(T)=1Z∑i=1Nεie−εiβS(T)=kBln⁡(Z)+ET![{\displaystyle {\begin{aligned}Z(T)&=\sum _{i=1}^{N}e^{-\varepsilon _{i}\beta }\\[6pt]E(T)&={\frac {1}{Z}}\sum _{i=1}^{N}\varepsilon _{i}e^{-\varepsilon _{i}\beta }\\[6pt]S(T)&=k_{\text{B}}\ln(Z)+{\frac {E}{T}}\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/964828553e88ca8a198609afcbb3dfb2e47d20e0)

Following the previous example, we choose a state with two levels and two particles. This leads to microstates _ε_1 = 0, _ε_2 = 1, _ε_3 = 1, and _ε_4 = 2.

Z(T)=e−0β+2e−1β+e−2β=1+2e−β+e−2βE(T)=0e−0β+2×1e−1β+2e−2βZ=2e−β+2e−2βZ=2e−β+2e−2β1+2e−β+e−2βS(T)=kBln⁡(1+2e−β+e−2β)+2e−β+2e−2β(1+2e−β+e−2β)T![{\displaystyle {\begin{aligned}Z(T)&=e^{-0\beta }+2e^{-1\beta }+e^{-2\beta }\\[3pt]&=1+2e^{-\beta }+e^{-2\beta }\\[6pt]E(T)&={\frac {0e^{-0\beta }+2\times 1e^{-1\beta }+2e^{-2\beta }}{Z}}\\[3pt]&={\frac {2e^{-\beta }+2e^{-2\beta }}{Z}}\\[3pt]&={\frac {2e^{-\beta }+2e^{-2\beta }}{1+2e^{-\beta }+e^{-2\beta }}}\\[6pt]S(T)&=k_{\text{B}}\ln \left(1+2e^{-\beta }+e^{-2\beta }\right)+{\frac {2e^{-\beta }+2e^{-2\beta }}{\left(1+2e^{-\beta }+e^{-2\beta }\right)T}}\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8d9faf1d4b889bebb08aaf851c802cf9142fb8e0)

The resulting values for S, E, and Z all increase with T and never need to enter a negative temperature regime.



 Bose–Einstein distribution and the Fermi–Dirac distribution approaches the [Maxwell–Boltzmann distribution](https://en.wikipedia.org/wiki/Maxwell%E2%80%93Boltzmann_statistics#Applicability "Maxwell–Boltzmann statistics") in the limit of high temperature and low particle density, without the need for any ad hoc assumptions


