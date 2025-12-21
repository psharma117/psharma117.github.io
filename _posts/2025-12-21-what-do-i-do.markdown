---
layout: post
title:  "What do I do?"
date:   2025-06-14 13:19:19 -0500
categories: everyone
---

<!--
Source - https://stackoverflow.com/a
Posted by nullromo
Retrieved 2025-12-20, License - CC BY-SA 4.0
-->

<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$']]
    }
  };
</script>


I have different ways of discussing my research with non-physicists, physics students, and physicists. 
So, I'm going to explain myself in three different ways accordingly. 
**As a standard disclaimer, any perspectives or statements here do not reflect anything/anyone other than my own thoughts and understanding. Any misunderstandings here are solely my own.**

# Non-Physicists 
I work on what's called the nuclear many-body problem.
My work lives in a small region of the atom - right at the center, as pictured here
<figure style="text-align: center; padding: 1em 0;">
  <img src="/assets/images/wiki_nucleus_atom.png" alt="Nucleus diagram" style="max-width: 100%; height: auto;" />
  <figcaption style="font-size: 0.85em; color: #555; margin-top: 0.5em;">
    Image by Wikimedia user Yzmo – CC BY-SA 3.0
  </figcaption>
</figure>


This means I'm trying to contribute to how we understand what happens when we have many protons and neutrons all interacting with each other at the center of atoms or in stars.
There are a variety of resolution scales that we think of nuclei in: 
- **Quarks and Gluons** are the things that make up all of the particles in a nucleus. 
The application to the many-body problem is primarily (to my knowledge) through a framework called Lattice QCD. 
- **Nucleons and Mesons** are perhaps the first thing you'd see if you looked up nuclei on the internet.
A *nucleon* is a lumped together term for a proton or a neutron.
This is a more "zoomed out" picture of what's happening in an atomic nucleus.
- **Densities and Currents** are a still more zoomed out picture, where we think of any individual nucleus as a blob of stuff (densities) that can jiggle around and flow (as currents) when we mess with it. 
This is the most "zoomed out" picture, and I engage with bridging it to the others. 

The name of the theoretical framework for the level of densities and currents is *Density Functional Theory (DFT)*. 
In a more ''zoomed in'' perspective, we would want to calculate (or approximate) the energy of each particle from every other particle.
This gets cumbersome and quite infeasible as the number of particles involved gets larger, like for heavier nuclei. 
In DFT we instead talk about the energy of the system in terms of (at bare minimum) a density of particles.

As a very simplified example of the distinction between zoom levels when describing the same system, I can think of the way individual H$_2$O molecules are interacting when I have water in a bucket, or I can just talk about the distribution of water at different points in the bucket. 
Thinking in terms of the H$_2$O molecules, I'd have to think about how the molecules interact with each other, how their bonds affect the basic attraction and repulsion that all charged particles experience.
I would have to find clever ways of using and obtaining information about what all the particles are doing at any instant in time.
I could also think of the collective variable: the distribution of the water in the bucket.
If we leave the water alone and it's allowed to just relax, we know it'll settle and form a cylinder with a flat top inside the bucket.
This is known as the *ground state* of the water. 
In this simple analogy, DFT says that if you have the correct shape that the water is distributed in while it's in its ground state, you can get all measurable properties of the system. 
To do something roughly like DFT on the water, we'd then need a good model of how water behaves, which accurately includes features such as water's surface tension (in case we put it in a container that it completely fills), its viscosity (if we poke the water, it doesn't stay dented for a while), and so on. 
The technical term for such a model is the Energy Density Functional (EDF). 
Slightly more specifically, the EDF is a rule that says: If you give me some description of the distribution of whatever you're describing, I'll tell you the energy associated with it.
Once I know how the system is distributed in the ground state, I can calculate anything I want about the properties of the system.
In the ground

As a reminder, the water bucket is a very simplified analogy to help me communicate the idea of changing your description based on how ``zoomed in'' you are since that's a crucial idea in my work.
The EDF tells us all the energies that we could get, but we don't know the correct EDF!
Informed by experimental findings, we can write down EDFs that we can make match data to good precision.
This is what's done currently, and it has worked pretty well at matching results that we measure, with some changes of numbers in the EDF to emphasize different features of different kinds of nuclei.
I'm working on improving EDFs at the level of the formulation.
Everything we write down in physics theory is an approximation, and EDFs are no exception.
To describe this idea better, it's once again helpful to use an analogy.

Let's say I wanted to calculate the circumference of a circle in order to perfectly wrap a ribbon around a disk or something like that.
Of course, anyone would just bring the disk to the ribbon, wrap the ribbon around the disk, and cut the right amount with this as a guide.
I simply want to use this scenario as a backdrop to illustrate the idea of what it means to approximate something in different ways.
A quick Google search tells us that the circumference of a circle with a diameter $D$ is $\pi\times D$.
Now, $\pi$ is an infinite decimal equal to 3.1415927... blah blah blah, so we cannot ever write down the exact circumference of any circle as a number with digits, but this does not matter in practice because we can get close enough to the exact circumference where the error does not matter.
For concreteness, let's say we have a circle with a diameter of 2 meters.
One way to approximate the length of ribbon I need is to say "eh, $\pi$ starts with 3, so I need 3$\times 2 = 6$ meters of ribbon."
Obviously, we're not going to get the exact amount of ribbon we need because we replaced $\pi$ with a nicer number - an approximation to $\pi$. 
We could improve on my approximation by including another digit: if we get $3.1\times 2 = 6.2$ meters of ribbon, we'll be closer to what we actually need.
But we could do other things too!
We can approximate the circle as a square with a side length of 2 meters, and get enough material to wrap around the square.
This will have me getting too much ribbon.
We can improve on this approximation by instead approximating the circle as a hexagon with a distance of 2 meters between opposite sides.
A still better approximation comes with treating it as an octogon with a distance of 2 meters between opposite sides.
Both of these schemes will eventually get to the right answer, perhaps at different rates and with different amounts of difficulty that may or may not help us with other aspects of whatever job has us playing with ribbon and disks.

Now, you might be thinking: why bother with all this guesswork? 
Just pull out your calculator, type $2\times \pi$, and be done with it.
This is in fact what we do when we have access to the exact (or precise enough) answer.
But for the nuclear many-body problem (and all of ongoing physics research!), _we don't have access to an exact answer!_
On the theoretical end of things where I work, we do not have an exact model of the nucleus that we can just pull up and say "Hey yeah let me get the structure of $^{47}$Ca with fries."
What we have are whatever information the experimentalists have brilliantly figured out how to measure in a lab or in space.
We have to then build a model that not only accurately matches those findings, but also predicts what else the experimentalists can find.
The exact answer is not accessible because the systems are so complicated, that to try to exactly calculate them on a computer would require more computational power, storage, and memory than what the whole universe could provide.
So, we must come up with approximations. 
These approximations should work well and should be systematically improvable.
You're only limited in your ribbon cutting adventures by how many digits of pi you have access to, you can keep improving it!
If we have 6.2 meters of ribbon and want to do better, we can just add another digit of $\pi$. 
If we want to do better still, another digit.
We know exactly what to do to improve our approximations: it's systematic.
In the nuclear many-body problem, we must formulate our approximations in more complicated ways because the problem is much more complicated.

With all of these ideas in mind, I can now succinctly answer the question posed by this article: What Do I Do?
I focus on elements of nuclear interactions and properties, and try to formulate systematically improvable approximations to calculate the observable collective features of nuclei to bridge pictures at the resolution of **Nucleons and Mesons** with the picture of **Densities and Currents**



















