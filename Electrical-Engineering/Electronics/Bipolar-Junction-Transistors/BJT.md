<h1 style="text-align:center;">Bipolar Junction Transistors | BJT</h1>

<h4>
First, we have the three regions of a Bipolar Junction Transistor (BJT): the
<strong>Emitter</strong>, <strong>Base</strong>, and <strong>Collector</strong>.
Each region has distinct characteristics that contribute to the transistor's
main function: controlling a large collector current using a much smaller base current.
</h4>

<center><h3 style="color:red;">Emitter</h3></center>

<p>
This region is heavily doped with charge carriers.
In an <strong>NPN</strong> transistor, it is heavily doped with electrons,
while in a <strong>PNP</strong> transistor, it is heavily doped with holes.
Its job is to inject these charge carriers into the Base.
</p>

<center><h3 style="color:red;">Base</h3></center>

<p>
The Base is extremely thin and lightly doped with the opposite type of semiconductor.
Because it is so thin, only a small number of charge carriers recombine inside it,
allowing most of them to reach the Collector.
This is why a small Base current can control a much larger Collector current.
</p>

<center><h3 style="color:red;">Collector</h3></center>

<p>
The Collector has the same semiconductor type as the Emitter but is less heavily doped.
It is physically larger than the Emitter because it must collect most of the charge carriers
coming from the Base and dissipate the heat generated during operation.
</p>

<blockquote style="color:#8B8000;">
<strong>Note:</strong> Throughout these notes, I treat electrons and holes as if they were two
different particles. In reality, holes are simply a convenient way to describe the absence of
electrons inside the semiconductor crystal, but thinking of them as separate carriers makes
the transistor much easier to understand.
</blockquote>

<figure>
<center>
<img src="https://circuitcrush.com/wp-content/uploads/BJT-Cross-Section.jpg"
width="300" alt="BJT Cross Section">
<figcaption>Figure 1</figcaption>
</center>
</figure>

<center><h2 style="color:red;">Its Function</h2></center>

<p>
To make an <strong>NPN transistor</strong> act as a switch, we first need to understand the
two PN junctions inside it and how they interact.
</p>

<h3>NPN Junctions</h3>

<p>
Let's start with the <strong>Emitter-Base junction</strong>.
Since it consists of two oppositely doped semiconductor materials, charge carriers diffuse
across the junction until an electric field is created. This electric field forms a
<strong>depletion region</strong> with a built-in potential that prevents any further diffusion.
</p>

<p>
To allow current to flow, this built-in potential must be reduced.
This is done by <strong>forward biasing</strong> the junction:
the positive terminal is connected to the P-type material (Base) and the negative terminal
to the N-type material (Emitter). As a result, the depletion region becomes narrower and
current can flow once the applied voltage is high enough.
</p>

<p>
If the polarity is reversed (<strong>reverse bias</strong>), the depletion region becomes wider,
preventing current flow except for a tiny leakage current.
</p>

<figure>
<center>
<img src="https://upload.wikimedia.org/wikipedia/commons/5/52/Pn-junction-equilibrium-graph.svg"
width="300" alt="PN Junction">
<figcaption>Figure 2</figcaption>
</center>
</figure>

<p>
The <strong>Collector-Base junction</strong> behaves similarly, but something interesting happens
when both junctions work together.
</p>

<h5>Case 1</h5>

<p>
If only the Base-Emitter junction is forward biased (or similarly only the Collector-Base
junction), then nothing particularly special happens—it simply behaves like a normal diode.
Current flows only if that junction is forward biased.
</p>

<h5>Case 2</h5>

<p>
If a voltage is applied only between the Collector and the Emitter, the transistor still
doesn't conduct any significant current.
</p>

<blockquote style="color:#8B8000;">
<strong>Learning Note:</strong><br>
I kept searching for about an hour trying to understand why this happens, but eventually
realized that I first need to study semiconductor physics. I was basically trying to learn
years of semiconductor theory in a couple of hours 😅. For now, I'll simply accept this fact
and come back to it once I understand semiconductor physics better.
</blockquote>

<h5>Case 3</h5>

<p>
Now things get interesting.
</p>

<p>
If the Collector-Emitter voltage is applied <strong>and</strong> the Base-Emitter junction is
forward biased, the Emitter injects electrons into the thin Base.
Because the Base is extremely thin and lightly doped, only a few electrons recombine there.
Most of them are swept into the Collector by the electric field created by the
reverse-biased Collector-Base junction.
</p>

<p>
This is where the transistor starts doing its magic:
a very small Base current allows a much larger Collector current to flow.
Increasing the Base current allows more electrons to reach the Collector,
which increases the Collector current even further.
</p>

<figure>
<center>
<img src="https://images.wevolver.com/eyJidWNrZXQiOiJ3ZXZvbHZlci1wcm9qZWN0LWltYWdlcyIsImtleSI6ImZyb2FzYS8xNzAyOTM1MTU2MDQzLTQ4LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6OTUwLCJmaXQiOiJjb3ZlciJ9fX0="
width="300" alt="NPN Transistor">
<figcaption>Figure 3</figcaption>
</center>
</figure>
