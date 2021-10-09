---
layout: post
title:  "A Funny Derivation of the SHM Period Formula with Minimal Calculus"
author: eyangch
tags:   ["Physics", "Physics 1", "SHM", "Simple Harmonic Motion", "Period", "Derivation"]
---

# A Funny Derivation of the SHM Period Formula with Minimal Calculus

## What is a SHM?

It is a simple harmonic oscillator, which means it is a system similar to a mass on a spring going back and forth. The equilibrium is the position the mass on the SHM is located to be at rest.

## The SHM Period Formula

$$T=2\pi \sqrt{\frac{m}{k}}$$

In this case, $$T$$ is the period, $$m$$ is the mass of the weight on the spring, and $$k$$ is the spring constant. The period is not dependent on amplitude, $$A$$. We will be trying to derive this formula.

## Hooke's Law

$$F = -kx$$

The restoring force, $$F$$, is the opposite of the spring constant $$k$$ times the displacement from equilibrium, $$x$$.

## Kinetic Energy Formula

$$KE = \frac{1}{2}mv^2$$

The kinetic energy of the object, $$KE$$, is half times the mass, $$m$$, times the velocity squared, $$v^2$$.

Recall that the formula for work is $$W=\Delta E = Fd = mad$$. Assuming everything is moving in one direction, we can write $$\Delta E = ma \Delta x$$. With the equation $$v_f^2 = v_i^2 + 2a\Delta x$$, we can rearrange to find that $$a \Delta x = \frac{v_f^2-v_i^2}{2}$$. Multiplying both sides by $$m$$ results in $$\Delta E = ma\Delta x = \frac{1}{2}v_f^2 - \frac{1}{2}v_i^2$$, so $$KE = \frac{1}{2}mv^2$$.

## Spring Potential Energy Formula

$$U = \frac{1}{2}kx^2$$

The potential energy of a spring, $$U$$, is half times the spring constant, $$k$$, times the displacement from equilibrium squared, $$x^2$$.

With $$W=Fd$$, we can determine the work by calculating the area under the force-distance graph from $$0$$ to $$x$$ (amount of energy spring system accumulates). Because $$F = -kx$$, the force varies proportionally with the displacement from equilibrium. Algebraically, we can calculate the area under the $$F = -kx$$ from $$0$$ to $$x$$ as a triangle to have a magnitude of $$\frac{1}{2}(kx)(x)$$, or, $$U = \frac{1}{2}kx^2$$.

This can be expressed as:

$$\int_0^x -kx \, \mathrm{d}x = -\dfrac{1}{2}kx^2$$

(scary!!!)

## A Formula for Displacement of SHM

$$x(t) = A \cos\left(\frac{2\pi}{T}t\right)$$

Why is this the displacement? idk its calculus stuff just trust me bro

$$A$$ is the amplitude, $$T$$ is the period, and $$x(t)$$ is the displacement of the SHM after $$t$$ seconds.

## Deriving the Period Formula

When the spring mass oscillating, the point in time when all of the energy in the system is kinetic energy would be when the mass is at the equilibrium point, and the point in time when all the energy is potential energy would be when the mass is furthest from the equilibrium point. We can write the following equation for velocity at equilibrium:

$$\frac{1}{2}kA^2 = \frac{1}{2}mv^2 \Rightarrow kA^2 = mv^2 \Rightarrow v = A\sqrt{\frac{k}{m}}$$

We also know that the slope of $$x(t)$$ at time $$t$$ is equal to $$v(t)$$, or the velocity. So, at equilibrium, the slope of $$x(t)$$ must equal $$A \sqrt{\frac{k}{m}}$$. Because the parent function, $$f(t)=\cos(t)$$, has a slope with a magnitude of $$1$$ at equilibrium ($$x(t)=0$$), we can transform $$f(t)$$ into $$x(t)$$ by altering the slope. First, we notice that both $$v$$ and $$x(t)$$ have a leading $$A$$ coefficient, we can write $$x(t) = Af(bt)$$. Since $$A$$ multiplies the slope of $$f(t)$$ by $$A$$ times at $$x(t)=0$$ and $$b$$ multiplies the slope of $$f(t)$$ by another $$b$$ times at $$x(t)=0$$, we know that:

$$Ab = A\sqrt{\frac{k}{m}} \Rightarrow b = \sqrt{\frac{k}{m}}$$

In $$x(t)$$, we know $$b = \frac{2\pi}{T}$$, so we can set our two equations for $$b$$ equal to each other and solve for $$T$$ to get us our period formula.

$$\frac{2\pi}{T} = \sqrt{\frac{k}{m}} \Rightarrow \boxed{T=2\pi \sqrt{\frac{m}{k}}}$$
