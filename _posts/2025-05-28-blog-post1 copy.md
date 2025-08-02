---
title: "Systems, System Norms, H-infinity, and Dissipation: Part 1"
date: 2025-05-28
permalink: /posts/2025/05/28/post1/
tags:
  - control
  - robust control
  - system
  - Lyapunov
math: true
---

What is a system? How can we characterize the system?

Its meaning can be drastically different for people working on, well, different systems. The word's usage is very broad and general indeed.

What we are interested in is, however, a specific set of equations that can describe any physical or digital processes with inputs, outputs, and in many cases, internal states.

An example is a simple process (simple as in the processes that can be described by a linear set of differential equations, or difference equations) like the following:

$$
\begin{align}
x_{k+1} &= Ax_{k} + Bw_{k} \\
z_{k} &= Cx_{k} + Dw_{k}
\end{align}
$$

where we use \\(x_{k}\\) to represent the "internal" state of the process, \\(w_{k}\\) the external input to the process, e.g., noise, disturbance, etc., and \\(z_{k}\\) the external output from the process, e.g., performance output.

In control theory, since we are interested in the special (controlled) inputs that we can "design" and "manipulate", we often write the controlled input (and use \\(u_{k}\\)) explicitly to distinguish from the uncontrolled input \\(w_{k}\\) that we assume given to us by nature, or difficult to model even if not from nature.

Hence, we often write the (linear) system as follows:

$$
\begin{align}
x_{k+1} &= Ax_{k} + B_{1}w_{k} + B_{2}u_{k} \\
z_{k} &= C_{1}x_{k} + D_{11}w_{k} + D_{12}u_{k}\\
y_{k} &= C_{2}x_{k} + D_{21}w_{k} + D_{22}u_{k}
\end{align}
$$

with \\(y_{k}\\) as the special "measurement" output (again different from \\(z_{k}\\), as we did for \\(u_{k}\\) to \\(w_{k}\\)).

One way to characterize the system is to examine its input-to-output effects. 
For example, how does the system amplifiy or attenuate the given input energy?
How sensitive is the system to the external input \\(w_{k}\\), for example?

To analyze these input-output relationships systematically, we have an useful construct called the transfer function, which is essentially a frequency-domain representation of the given system, and characterizes how a system transforms inputs at a given frequency into outputs. For our linear time-invariant system, we can define the transfer function from input \\(w_{k}\\) to output \\(z_{k}\\) as:

$$G(z) = C_1(zI - A)^{-1}B_1 + D_{11}$$

This transfer function \\(G(z)\\) encodes all the information about how the system maps the input signal to the output signals.
But knowing the transfer function is just the first step; we need ways to quantify how "large" or "small" this input-output effect is.
This is where the concept of the system norm become useful. We have many different norms that capture different notions of system "size" or "gain".

In particular, the \\(H_\infty\\) norm measures the "worst-case amplification" of the system, the maximum factor by which the system amplifies the input energy (across all possible frequencies).

Mathematically, the \\(H_\infty\\) norm can be defined as:
$$\|G\|_{H_\infty} = \sup_{\omega} \sigma_{\max}(G(e^{j\omega}))$$

where \\(\sigma_{\max}\\) denotes the largest singular value. This norm tells us the maximum gain the system can induce, which is crucial for characterizing the "robustness" of the system to disturbances.

Rather than computing this norm directly from the transfer function, and computing its singular values as above, we can also use an alternative characterization, which utilizes the concept of dissipation, and is conceptually more intuitive, at least to me.

To cut to the chase, we have the following alternative definition of the \\(H_\infty\\) norm:

$$\|G\|_{H_\infty} = \sup_{\substack{w \neq 0 \\ w \in \ell_2}} \frac{\|z\|_{\ell_2}}{\|w\|_{\ell_2}} < \gamma$$

for some \\(\gamma > 0\\). This is equivalent to asking whether 

$$\|z\|_{\ell_2} \leq \gamma \|w\|_{\ell_2}$$

for all non-zero inputs \\(w \in \ell_2\\).

As we shall see soon, this is rooted in the dissipation ineqaulity. 

For sequences over time, this condition translates to:
$$\sum_{k=0}^{\infty} z_k^T z_k \leq \gamma^2 \sum_{k=0}^{\infty} w_k^T w_k$$

We can rewrite this constraint by introducing the point-wise supply rate:
$$s_{k} = \gamma^2 w_k^T w_k - z_k^T z_k$$. The supply rate \\(s_{k}\\) represents the "net energy" being supplied to the system at time \\(k\\).

Here is where the dissipation inequality comes in.

Consider a storage function \\(V(x) \geq 0\\) representing the internal energy (note that in many physical systems, the concept of energy is naturally characterized by quadratic functions, e.g., kinetic energy, potential energy) stored in the system state. The dissipation inequality states:

$$V(x_{k+1}) - V(x_k) \leq s_{k} = \gamma^2 w_k^T w_k - z_k^T z_k$$

This inequality has a nice physical meaning, i.e., the first law of theremodynamics:

> "The change in internal energy of a system equals the energy added to the system minus the work done by the system."

Here, \\(\gamma^2 w_k^T w_k\\) represents energy injection, \\(z_k^T z_k\\) represents energy extraction (work done by the system), and \\(V(x_{k+1}) - V(x_k)\\) captures the change in stored energy.


Considering the dissipation, the energy losses due to inefficiencies, e.g., friction, damping, etc., it states that the increase in internal energy is less than or equal to the net energy injected into the system.

In the next, we will use this to write the Bounded Real Lemma, and characterize the system via \\(H_\infty\\) norm.