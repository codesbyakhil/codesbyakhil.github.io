---
title: "Setting up this site"
subtitle: "A public lab notebook — and a quick test that equations and Fortran render properly."
tags: [meta]
---

This site is meant to work like a lab notebook with the door open: research progress on
the [Research]({{ '/research/' | relative_url }}) page, short dated updates on the
homepage, and longer notes here when something is worth writing down properly.

Since most of what I might write about involves equations, here is the rendering test.
The phase-mass conservation equation from the six-equation two-fluid model I work with:

$$
\frac{\partial}{\partial t}\left(\alpha_k \rho_k\right)
+ \nabla \cdot \left(\alpha_k \rho_k \, \mathbf{u}_k\right) = \Gamma_k
$$

where $$\alpha_k$$, $$\rho_k$$, and $$\mathbf{u}_k$$ are the volume fraction, density,
and velocity of phase $$k$$, and $$\Gamma_k$$ is the interphase mass-transfer term.
Inline math works too: the shedding regime I simulate sits at
$$\mathrm{Re} = 100\text{–}300$$.

Code blocks get the same treatment. A crude way to estimate the shedding frequency from
a lift-coefficient history — counting upward zero crossings:

```fortran
! shedding frequency from upward zero crossings of C_L(t)
nzero = 0
do i = 2, nt
   if (cl(i-1) < 0.0d0 .and. cl(i) >= 0.0d0) nzero = nzero + 1
end do
f_shed = dble(nzero) / t_total
st     = f_shed * d / u_inf      ! Strouhal number
```

If you can read both of those clearly, the pipeline works. More substantial posts to
follow — feel free to delete this one once the site is live.
