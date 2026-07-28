# Bipolar Junction Transistors (BJT)

The **Bipolar Junction Transistor (BJT)** is a semiconductor device used to control a large current using a much smaller current. It consists of **three regions**: the **Emitter**, **Base**, and **Collector**. Each region has unique physical characteristics that contribute to the transistor's operation.

---

## Emitter

The **Emitter** is heavily doped with charge carriers.

- In an **NPN transistor**, it is heavily doped with **electrons**.
- In a **PNP transistor**, it is heavily doped with **holes**.

Its primary job is to **inject charge carriers into the Base**.

---

## Base

The **Base** is the thinnest region of the transistor and is **lightly doped**.

Because it is so thin, only a small number of charge carriers recombine inside it. Most of the carriers injected by the Emitter are able to pass through the Base toward the Collector.

A small current through the Base controls a much larger current flowing between the Collector and the Emitter.

---

## Collector

The **Collector** is doped with the same type of semiconductor as the Emitter but is **less heavily doped**.

Its purpose is to collect nearly all of the charge carriers that travel through the Base. It is also physically larger than the other regions to allow it to dissipate heat more effectively.

> **Note**
>
> Throughout these notes, electrons and holes are treated as if they were two different particles. Physically, holes are simply a convenient way to describe the absence of electrons inside the crystal, but treating them as independent carriers makes understanding semiconductor devices much easier.

---

<p align="center">
<img src="https://circuitcrush.com/wp-content/uploads/BJT-Cross-Section.jpg" width="300">
</p>

<p align="center"><b>Figure 1 — BJT Cross Section</b></p>

---

# Operating Principle

To understand how an **NPN transistor** works, we first need to understand the two PN junctions inside it.

- **Emitter-Base Junction (EB)**
- **Collector-Base Junction (CB)**

Each junction behaves like a PN diode.

---

## The Emitter-Base Junction

The Emitter is an **N-type** semiconductor while the Base is **P-type**.

When these materials are joined together, electrons and holes diffuse into the opposite material until an electric field forms between them. This creates a **depletion region** with a built-in potential that prevents further diffusion.

Current can only flow if this built-in potential is reduced.

### Forward Bias

The junction is forward biased when

- Positive voltage is applied to the Base.
- Negative voltage is applied to the Emitter.

This reduces the depletion region and allows current to flow once the applied voltage is sufficiently large.

### Reverse Bias

The junction is reverse biased when the polarity is reversed.

The depletion region widens, preventing current flow except for a very small leakage current.

---

<p align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/5/52/Pn-junction-equilibrium-graph.svg" width="300">
</p>

<p align="center"><b>Figure 2 — PN Junction</b></p>

---

The **Collector-Base Junction** behaves exactly like another PN junction. The interesting behavior appears when both junctions operate together.

---

## Case 1 — Only the Base-Emitter Junction is Forward Biased

If only the Base-Emitter junction is forward biased, it behaves exactly like a diode.

Current flows through the Base-Emitter junction, but there is no significant Collector current.

---

## Case 2 — Only the Collector-Emitter Voltage is Applied

Applying a voltage only between the Collector and the Emitter does **not** make the transistor conduct.

At first this may seem surprising.

The reason involves semiconductor physics and the behavior of the depletion regions inside the transistor. A deeper explanation requires understanding carrier transport and electric fields inside semiconductor materials.

> **Learning Note**
>
> I searched for a complete explanation here but realized that I first need a stronger background in semiconductor physics. For now, I will simply accept this behavior and revisit it later.

---

## Case 3 — Normal Active Operation

Now suppose

- A voltage is applied between the Collector and the Emitter.
- The Base-Emitter junction is forward biased.

The forward-biased Base-Emitter junction injects a large number of electrons into the thin Base.

Since

- the Base is extremely thin,
- only lightly doped, and
- the Collector-Base junction is reverse biased,

most of these electrons are swept into the Collector by the electric field inside the Collector-Base depletion region.

This creates a large Collector current.

A small increase in the Base current allows more charge carriers to enter the Base, producing a much larger increase in the Collector current.

This is the fundamental operating principle of a BJT.

---

<p align="center">
<img src="https://images.wevolver.com/eyJidWNrZXQiOiJ3ZXZvbHZlci1wcm9qZWN0LWltYWdlcyIsImtleSI6ImZyb2FzYS8xNzAyOTM1MTU2MDQzLTQ4LmpwZyIs width="300">
</p>

<p align="center"><b>Figure 3 — NPN Transistor in Active Region</b></p>

---

# Summary

- The Emitter injects charge carriers.
- The Base controls how many carriers pass through.
- The Collector collects nearly all of those carriers.
- A small Base current controls a much larger Collector current.
- The Base-Emitter junction must be forward biased for normal transistor operation.
- The Collector-Base junction is reverse biased during active operation.
