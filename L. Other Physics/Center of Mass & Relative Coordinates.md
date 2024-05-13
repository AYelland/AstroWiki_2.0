---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---

Considering a set of particles of mass ($m_{1}$, $m_{2}$, $\dots$) with positions ($\vec{r}_{1}$, $\vec{r}_{2}$, $\dots$) respectively.

## Total Mass

The sum of individual masses ($m_{1}$, $m_{2}$, $\dots$) yield the **total mass** ($M$).

$$
M = \sum_{i} m_{i} = m_{1} + m_{2} + \dots
$$

## Reduced Mass

The product of individual masses ($m_{1}$, $m_{2}$, $\dots$) divided by the total mass ($M$) yield the **reduced mass** ($\mu$).

$$
\mu = \frac{\prod_{i} m_{i}}{\sum_{j} m_{j}} = \frac{m_{1} m_{2} \dots}{m_{1} + m_{2} + \dots} = \frac{m_{1} m_{2} \dots}{M}
$$

## Center-of-Mass Position

The weighted average of the position vectors ($\vec{r}_{1}$, $\vec{r}_{2}$, $\dots$) using the associated masses ($m_{1}$, $m_{2}$, $\dots$) yields the **center-of-mass position** ($\vec{R}$).

$$
\vec{R} = \frac{\sum_{i} m_{i} \vec{r}_{i}}{\sum_{j} m_{j}} = \frac{m_{1} \vec{r}_{1} + m_{2} \vec{r}_{2} + \dots}{m_{1} + m_{2} + \dots} = \frac{m_{1} \vec{r}_{1} + m_{2} \vec{r}_{2} + \dots}{M}
$$

## Center-of-Mass Momentum

The total mass of the system ($M$) multiplied by the velocity of the center-of-mass ($\dot{\vec{R}}$) yields the **center-of-mass momentum** ($\vec{P}$). As it turns out, this is also just the sum of the individual mass's momentums ($\vec{p}_{1}$, $\vec{p}_{2}$, $\dots$).

$$
\vec{P} = M \dot{\vec{R}} = M \left(\frac{m_{1} \dot{\vec{r}}_{1} + m_{2} \dot{\vec{r}}_{2} + \dots}{M}\right) = m_{1} \dot{\vec{r}}_{1} + m_{2} \dot{\vec{r}}_{2} + \dots = \vec{p}_{1} + \vec{p}_{2} + \dots
$$

## Relative Position

The vector difference between the positions of two masses ($\vec{r}_{1}$ and $\vec{r}_{2}$) yields the **relative position** of one mass with respect to the other.

$$
\vec{r} = \vec{r}_{1} - \vec{r}_{2}
$$

## Relative Momentum

The reduced mass of the system ($\mu$) multiplied by the relative velocity ($\, \dot{\vec{r}} \,$) yields the **relative momentum** ($\, \vec{p} \,$).

$$
\vec{p} = \mu \dot{\vec{r}} = \mu ( \dot{\vec{r}}_{1} - \dot{\vec{r}}_{2} )
$$