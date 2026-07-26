# Bipolar Junction Transistors | BJT
<h4>First we got the three layers --> Emitter, Base and Collector. These regions have some distinct characters that contribute to the main function of the transistor, which is controlling current in a circuit without disturbing anything in the circuit.</h4>
<center><h3 style = "color: red;">Emitter</h3></center>
<p>This part is heavily doped either with Electrons or Holes, which means it got excess of free electrons, which will help the electrons to go from it to the base or the collector</p>
<center><h3 style = "color: red;">Base</h3></center>
<p>This part is extremely thin and lightly doped with the opposite of Emitter and Collector, which will make it easy to control the collector current through the base and the emitter Potential Difference</p>
<center><h3 style = "color: red;">Collector</h3></center>
<p>This part is heavily doped with the same type as the emitter but less doped than it, the geometry of this part contributes to the efficiency of the transistor, because it helps catch most of the electrons or the holes coming from the base and dissipate heat !</p>
<blockquote style = "color: #8B8000;">Note: I am dealing with the Holes and Electrons as two separate particles but, in fact, it is just Electrons in action. But I could still treat them like this ;)</blockquote>
<figure>
<center>
<img src="https://circuitcrush.com/wp-content/uploads/BJT-Cross-Section.jpg" width ="300" alt="BJT junction">
<figcaption>Figure 1</figcaption>
</center>
</figure>
<center><h2 style= "color: red">Its Function</h2></center>
<p>
To make NPN transistor act as a switch in a circuit, First we need to know the correct way to connect a transistor and to do so we'll look at the NPN junctions and see how they interact.<br>
<h3>NPN junctions:</h3>
<p>Let's take the emitter-base junction, it contains two opposite doped crystals and that creates a potential difference between them. Its configuration is that the emitter have lots of electrons and the base has more holes so they immigrate into the opposite crystal until creating an electric field, which results in a built-in potential across the depletion region that is high enough to stop any further immigration. In order to conduct current, this potential difference must be first opposed, to do so the applied voltage is then applied in a way that decreased this potential difference <strong>(Forward Biased)</strong> in which the positive is connected to the P-type (Base) and the negative is connected to the N-type (Emitter), which will decrease the Depletion Region and conduct current if the applied voltage is high enough. But if it was the other way <strong>(Reverse-Biased)</strong> then the depletion region will increase and no current is conducted.
<figure>
<center>
<img src="https://imgs.search.brave.com/AbCCyduHb6k8jKfFrW7sJRAGsj2DERiEsqU9VlyA2TY/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly91cGxv/YWQud2lraW1lZGlh/Lm9yZy93aWtpcGVk/aWEvY29tbW9ucy81/LzUyL1BuLWp1bmN0/aW9uLWVxdWlsaWJy/aXVtLWdyYXBoLnN2/Zw" width ="300" alt="NP junction" >
<figcaption>Figure 2</figcaption>
</center>
</figure>
As for the collector-base junction it behaves the same, But something interesting happens when we combine them.
<h5>Case 1</h5>
When the applied voltage is just between the base-emitter junction (the same goes for collector-base junction), u kinda didn't do nothing new a current will pass, if only forward-biased, as expected and thats it !!!
<h5>Case 2</h5>
When the applied voltage is just between the collector-emitter, here it gets a bit interesting and the transistor doesn't conduct any current, which is honestly i don't understand yet, I kept searching for an hour to find a convincing answer but I found out that I need to study semiconductor physics, which I was trying to understand in a couple of hours ;) it's literally IMPOSSIBLE, so I will just take it for a fact for now :)
<h5>Case 3</h5>
When the applied voltage is across the emitter-collector and there is a potential difference between the emitter-base junction (Forward-Biased) to overcome the depletion region and conduct current, and for the fact that the base is extremely thin and lightly doped the electrons rush toward the collector and the transistor actually conducting Bingo !! that's not all, u could adjust the base voltage to further overcome the depletion region and even more current through the collector, and the crazy thing is u only need a small change in voltage between the base-emitter to make the collector current even bigger.
<figure>
<center>
<img src="https://imgs.search.brave.com/opSNtiz62e92lIHYyy2Lmod-cbAjE3vjwR2C9kmEoh0/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pbWFn/ZXMud2V2b2x2ZXIu/Y29tL2V5SmlkV05y/WlhRaU9pSjNaWFp2/YkhabGNpMXdjbTlx/WldOMExXbHRZV2Rs/Y3lJc0ltdGxlU0k2/SW1aeWIyRnNZUzh4/TnpBeU9UTTFNVFUy/TURRekxUUTRMbXB3/WnlJc0ltVmthWFJ6/SWpwN0luSmxjMmw2/WlNJNmV5SjNhV1Iw/YUNJNk9UVXdMQ0pt/YVhRaU9pSmpiM1ps/Y2lKOWZYMD0" width ="300" alt="NPN transistor" >
<figcaption>Figure 3</figcaption>
</center>
</figure>
</p>