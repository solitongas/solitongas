---
title: Integral equation of the first kind
date: '2022-02-09'
slug: integral-equation-of-the-first-kind
categories: [integral equation, complex analysis, mathematical physics]
tags: [Fredholm equation, potential theory, capacity, ]
subtitle: ''
summary: ''
authors: [admin]
lastmod: '2022-02-09T10:37:03-05:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

# Background
Integral equations play important role in mathematical physics. In this short note, we are going to discuss a class of integral equation of the first kind. My motivation to study those equations is from soliton gas, where the nonlinear dispersion relation is as follows:
$$\int_\Gamma g(z,w)u(w)|dw|+\sigma(z)u(z)=\phi(z),\quad z\in \Gamma$$

where $\Gamma$ is some simple smooth rectifiable curve in $\mathbb{C}^+$ and kernel $g(z,w)=\log\left|\frac{z-\bar w}{z-w}\right|$ is so-called Green kernel (i.e. it is the Green function to the Direchlet problem on the upper half plane.). The case when $\sigma\equiv 0$ is referred to as soliton condensate. As one can immediately see, the equation becomes Fredholm equation of the first kind. It is well-known that integral equation of the first kind is (in general) ill-posed in the sense of Hadamard. Here we are going to consider a slightly different equation:
$$\int_{\Gamma}\log|w-z|^{-1} u(w)|dw|=f(z),\quad z\in \Gamma.$$

And we will consider the uniqueness of the equation using classical potential theory. Then we will use a method introduced by Yan&Sloan to solve the equation explicitly.

# Potential theory and uniqueness

Let's first introduce some definitions from classical complex analysis. All the definitions and theorems can be found on Hille's book.

**Definition 1.**  Let $\mu$ be a probability measure supported in $\Gamma$ (i.e. $\mu(\Gamma)=1$.), the **logarithmic potential** is
$$U^{\mu}(z)=-\int_\Gamma \log\left|z-w\right|d\mu(w),\quad z\in \mathbb{C}.$$

**Definition 2.** The **energy** is defined as
$$I(\mu)=\int U^{\mu}(z) d\mu(z).$$

**Definition 3.** The **capacity** of a compact set $\Gamma$ is defined as 
$$C_\Gamma=e^{-V_\Gamma}=\exp{(-\inf_{\mu\in M(\Gamma)}I(\mu))},$$ where $V_\Gamma$ is so-called **Robin constant**.

**Definition 4.** A **charge** is a signed measure, which always has the decomposition as $\sigma=\sigma_+-\sigma_-$, where $\sigma_\pm$ are called positive and negative part of the charge. And we denote the space of charge with finite energy as $S(\Gamma)$.

\begin{equation}
hhh
\end{equation}