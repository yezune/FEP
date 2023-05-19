# A Free Energy Principle for A Particular Physics

__Karl Friston__

*The Wellcome Centre for Human Neuroimaging, UCL Queen Square Institute of Neurology, London, UK WC1N 3AR. Email: k.friston@ucl.ac.uk
(This work is under consideration for publication by The MIT Press)*

## Abstract

This monograph attempts a theory of every ‘thing’ that can be distinguished from other ‘things’ in a statistical sense. The ensuing statistical independencies, mediated by Markov blankets, speak to a recursive composition of ensembles (of things) at increasingly higher spatiotemporal scales. This decomposition provides a description of small things; e.g., quantum mechanics – via the Schrödinger equation, ensembles of small things – via statistical mechanics and related fluctuation theorems, through to big things – via classical mechanics. These descriptions are complemented with a Bayesian mechanics for autonomous or active things. Although this work provides a formulation of every ‘thing’, its main contribution is to examine the implications of Markov blankets for self organisation to nonequilibrium steady-state. In brief, we recover an information geometry and accompanying free energy principle that allows one to interpret the internal states of something as representing or making inferences about its external states. The ensuing Bayesian mechanics is compatible with quantum, statistical and classical mechanics and may offer a formal description of lifelike particles.

**Key words**: *self-organisation; nonequilibrium steady-state; active inference; active particles; free energy; entropy; random dynamical attractor; autopoiesis; Markov blanket; Bayesian; variational.*

## Introduction

This monograph attempts a theory of every ‘thing’ – in a tongue in cheek way – starting from the premise that a ‘thing’ is distinguishable from something else and from no ‘thing’. Its ambition is to validate a formulation of dynamical systems by appealing to constructs in physics (e.g., quantum, statistical and classical mechanics) and then use the ensuing formulation to derive an account of self-organisation within the same framework[^note-1]. Our starting point is a definition of things in terms of systems that possess an invariant measure; namely, weakly mixing systems that possess an attracting set. The description of such systems usually starts using the formalism of random dynamical systems; for example, the flow or dynamics of systemic states based on random differential equations (e.g., a Langevin equation). This is where the current treatment starts – and then stops. It stops by asking some obvious questions; like, what are states and where do random fluctuations come from? These questions lead to even simpler questions; namely, if we are dealing with the states of something, what is the thing that possesses those states – and how does one distinguish anything from something else? The answers to these questions lead to a theory of everything in a literal sense.

[^note-1]: This paper was written as an autodidactic exercise to ensure the author’s intuitions played out over complementary formulations in statistical physics. The result is a long, over inclusive paper that tries to adopt conventions from different fields (which the author is not expert in), while emphasizing common themes.

To address the nature of things, we start by asking how something can be distinguished from everything else. In pursuing a formulation of self-organisation, we will call on the notion of conditional independence as the basis of this separation. More specifically, we assume that for something to exist it must possess (internal or intrinsic) states that can be separated statistically from (external or extrinsic) states that do not constitute the thing. This separation implies the existence of a Markov blanket; namely, a set of states that render the internal and external states conditionally independent. The existence of things (i.e., internal states and their blanket) further implies a partition of the Markov blanket into active and sensory states – that are not influenced by external and internal states, respectively. This may sound a bit arbitrary; however, this is the minimal set of conditional independencies – and implicit partition of states – that licenses talk about things (that possess states). Specifically, it provides a partition that constitutes the ‘self’ in self-organisation. The subsequent sections tackle the next obvious question: what are things? At this point, we deploy the Langevin formulation of random dynamical systems as an ansatz that is recursively self-verifying, when considered in the light of Markov blankets. In brief, the formulation on offer says that the states of things (i.e., particles) comprise mixtures of blanket states, where the Markov blanket surrounds things at a smaller scale. Effectively, this eludes the question “what is a thing?” by composing things from the Markov blanket of smaller things. By induction, we have Markov blankets all the way down, which means one never has to specify the nature of things.

More specifically, we will see that the Langevin formulation of dynamics – at any given spatiotemporal scale – can be decomposed into an ensemble of Markov blankets. These blanket states have a dynamics at a higher scale with exactly the same (Langevin) form as the dynamics of the original scale. When lifting the dynamics from one scale to the next, internal states are effectively eliminated, leaving only slow, macroscopic dynamics of blanket states. These become the states of things at the next level, which have their own Markov blankets and so on. The endpoint of this formalism is a description of everything at progressively higher spatial and temporal scales. The implicit separation of temporal scales is used in subsequent sections to examine the sorts of dynamics, physics or mechanics of progressively larger things.

This monograph comprises 12 sections organised into three parts. The first part establishes some basic results, the second part applies these results to limiting cases of dynamical systems to recover quantum, statistical and classical mechanics. The third part considers the special case of active or autonomous systems, in terms of a Bayesian mechanics for particles with internal states that ‘matter’ for their behaviour.

Part One: The first section is a foundational treatment that introduces some constraints on the dynamics of Markov blankets that possess measurable characteristics. The constraint of measurability – or possessing an invariant measure over sufficiently long periods of time – allows one to express the flow of states as a function of their non-equilibrium steady-state (NESS) density[^note-2]. The relationship between flow and the NESS density follows in a straightforward way from the Fokker Planck formulation of density dynamics and, in particular, its eigensolution. The interesting results here are the dependencies – implicit in the system’s equations of motion – that inherit from Markov blankets at nonequilibrium steady-state. The ensuing, relatively straightforward lemma and corollaries concerning marginal flows and conditional independencies then form the basis for emergent behaviours in subsequent sections. The second section looks at various ways in which one can characterise density dynamics in terms of symmetry breaking and self-organisation. This section uses information theory and geometry to characterise different sorts of self-organisation to nonequilibrium steady-state. The third section provides an illustration of self-organisation, using numerical analyses of a particular system (a synthetic primordial soup based on ensemble of Lorenz systems). This system is used throughout the monograph to illustrate how one can take complementary perspectives on the same dynamics. The fourth section considers the behaviour of this (Langevin) formulation of Markov blankets at nested scales. In brief, we assume that as one ascends to higher scales, random and intrinsic fluctuations are progressively suppressed, resulting in a move from dissipative dynamics – that are dominated by random fluctuations – through to large systems whose conservative dynamics are dominated by divergence-free flow.

[^note-2]: NESS could also be an acronym for Nearly Ergodic Steady-State in weakly mixing systems. As observed by my young colleague Brennan Klein, nonequilibrium steady-state puts the “ness” in “thingness” (From Middle English -nes, -nesse: appended to adjectives to form nouns meaning “the state of being”). We will argue later that any ‘state of being’ rests upon a NESS.

Part Two: Section 5 considers the very small in terms of quantum mechanics. This section derives the Schrödinger wave equation using the relationship between a particle’s flow and the NESS density established in the first section. The trick here is to express or factorise the NESS density in terms of (complex) roots that play the role of a wave function. Section 6 then considers the collective behaviour of small things in terms of ensemble dynamics and stochastic thermodynamics. Our focus here is on linking the dissipative dynamics of ensembles to established results in statistical mechanics; namely, the laws of thermodynamics and related fluctuation theorems such as the Jarzynski equality. We then turn to the physics of big things in the limit of small amplitude random fluctuations. This limit allows us to write down equations of motion in terms of a classical Lagrangian or Hamiltonian, leading to classical mechanics, Newtonian laws of motion and Maxwell's equations.

Part Three: Having cast quantum, statistical and classical mechanics as limiting cases of the density dynamics of inert particles, we turn to the ontology of big things – whose internal states cannot be ignored – that show autonomous behaviour (e.g., large active particles like ourselves). Section 8 asks why one might attribute representational or inferential capacities to biological self-organisation. In other words, how notions like the good regulator theorem (Conant and Ashby, 1970) and the Bayesian brain hypothesis (Helmholtz, 1878 (1971); Knill and Pouget, 2004) could be substantiated in terms of a sentient physics. The argument here is fairly straightforward: namely, that the internal states of a system encode probabilistic beliefs about external states that cause sensory impressions on the Markov blanket – and are caused by the influence of active states on external states. This section provides a formal basis for an information geometry and attending free energy principle that describes autonomous things (e.g., cells or brains) as inferring the causes of actively sampled sensations. Here, we pursue a variational theme by showing how variational Bayes (Beal, 2003) is an emergent property of certain kinds of particles, leading to a form of Bayesian mechanics. Section 9 illustrates a particular inference using numerical analyses of the synthetic soup from Part One (and a virus like denizen). Section 10 then considers active states and agency in terms of corollaries of the free energy principle based upon an integral fluctuation theorem and expected free energy. The penultimate section considers the ensuing active inference in light of previous (thermodynamic) treatments. We conclude with a brief discussion of the relationships between quantum, stochastic, classical and Bayesian mechanics.


## Part 1: the setup
### Something or nothing

The *“Siphonaptera”* is a nursery rhyme, sometimes referred to as Fleas:
*Big fleas have little fleas,
Upon their backs to bite 'em,
And little fleas have lesser fleas,
and so, ad infinitum.*

This nicely frames one approach to the question of ‘what is a thing?’ by appealing to an infinite regress in which the question goes away. This deflationary account[^note-3] says that the states of things are constituted by their Markov blanket, while the Markov blanket comprises the states of smaller things with Markov blankets within them – and so on ad infinitum. This appeal to blankets ‘all the way’ down offers a recursive definition of everything – at separable spatial and temporal scales – that are unpacked in Section 4, using notions from the renormalisation group. The idea of blankets all the way down (and up) suggest that there is no privileged scale, other than the scale that ‘matters’ for a thing in question. In the final sections, we will see that to ‘matter’ means there is an information geometry in play at certain scales, which afford autonomous and itinerant dynamics but are sufficiently large to suppress random fluctuations.

[^note-3]: An account that might also dissolve the prime mover (Latin: primum movens), advanced by Aristotle as a primary cause of all motion in the universe. In Book 12 (Greek "Λ") of his Metaphysics, Aristotle describes the prime mover as being perfectly beautiful, indivisible, and contemplating only the perfect contemplation: itself contemplating.

To foreshadow a more technical description, the basic story can be illustrated with a common-sense example. Imagine a solar system whose physics (i.e., dynamics or flow) is described sufficiently by the position, velocity and irradiation of heavenly bodies. These quantities constitute ensemble averages of each body’s surface (i.e., Markov blanket) with internal states fluctuating beneath. Now let us descend a scale and focus on a particular
planet (e.g., Earth). At this scale, the meteorological flows and geography of the planet’s surface now constitute an appropriate level of description with many (internal) microscopic states lying below. Now assume we have zoomed in to a city and can access these microscopic states that transpire to be the ebb and flow of commuters during the daily cycle of a metropolis. Now we come down a further level and appreciate that each element, previously contributing to the average behaviour of commuters, is an individual or entity with its own Markov blanket; namely, an embodied brain. At this level of description, the delicate and structured fluctuations of the inner workings of the brain are hidden behind the Markov blanket and yet, if we zoom in further, now become the Markov blankets of neuronal elements and processes that have been coordinating commuter behaviour. Here, the Markov blanket corresponds to a cell surface that itself surrounds intrinsic or internal intracellular processes; namely, exchange among intracellular organelles with their own Markov blankets. One could imagine going further and further through macromolecules down to atomic and subatomic levels. At each stage, we find a sufficient level of description according to the states of an ensemble that present themselves for engagement with – and coupling to – the Markov blanket of things at the level in question. Crucially, beneath (or sequestered behind) each Markov blanket are intrinsic or internal states that themselves are constituted by (mixtures of) ensembles of blanket states. In what follows, we will retell this story (from the bottom up), trying to show why these hierarchical levels of description are a necessary consequence of any (weakly mixing) random dynamical system that possess Markov blankets. However, first, we consider some preliminaries and background material that will be necessary to connect the different perspectives adopted in subsequent sections.

#### Some preliminaries

This section can be read as a foundational (introductory) treatment of physics. It is not rigorous but is sufficient to convey the basic ideas. To unpack some of the assertions and lemmas, each section is accompanied by numerical examples and comprehensive descriptions in the figure legends [^note-4]. The numerical analyses illustrate various phenomena using stochastic chaos based on a single Lorenz system (Lorenz, 1963) – or an ensemble of Lorenz systems, dressed with blanket states, to simulate active matter. These examples try to emphasise that, although the maths may look complicated, it describes sensible, emergent phenomena.

[^note-4]: These numerical analyses serve two purposes. First, they show how one can characterise the same system from complementary perspectives. For example, one can treat a system as a small particle (e.g., an electron), in terms of quantum mechanics; or we can treat it as an ensemble of particles (e.g., a gas), to examine its statistical mechanics; or we can treat it as a blob of mass (e.g., a ball) in some active medium and describe its response in terms of classical mechanics. In Part Three, we will take this further and look at autonomous behaviour; namely, how one part of a system actively infers or ‘measures’ another. The second purpose is more pedagogical (for biological readers); in the sense that the simulations dispel any mysticism surrounding high end physics. In short, all the mechanics considered in this monograph lend themselves to straightforward and intuitive numerical analyses that allow one kind of mechanics to be understood in relation to the others.

The mathematical notation is largely standard: the section on quantum mechanics will occasionally use the Dirac notation and the section on statistical mechanics follows (Seifert, 2012). Occasionally, we will use the (Einstein) summation convention when dealing with tensors. An exception to standard notation is the use of boldface variables; where $x \in X$ denotes a (generalised) coordinate in phase or state-space, while $x \in X$ denotes the expected or most likely value. $x(a)$ will denote an expectation, conditioned on a variable $a$. Boldface capital letters $X$ will denote operators. For clarity, functional derivatives and integrals involving time are expressed in terms of orbits, trajectories or paths $x[\tau]={x(\tau):\tau\in[0,t]}$ , where a value at time $\tau$ is denoted by $x(\tau)\equiv x_\tau$. We will also be dealing with time-dependent probability densities $p(x,\tau) \equiv p_{\tau}(x{\tau})$ that have stationary or steadystate solutions $p(x,\infty) \equiv p(x)$ in the limit $\tau \to \infty$; similarly, for their negative log density or surprisal $\Im (x,\tau) \equiv \Im _{\tau} (x_{\tau}) = −\ln \space p(x,\tau)$. For ease of reference, a glossary of terms and expressions is provided at the end of the monograph. Most of what follows rests on three equivalent and complementary descriptions of stochastic dynamics; the Langevin equation, path integral formulation and Fokker Planck equation.

**Langevin dynamics**: this formulation expresses the dynamics of systemic states $x(\tau)$  (i.e., states of some system) in terms of a state-dependent flow and some random fluctuations  $\omega (\tau)$:

$$
\begin{equation}\tag{1.1}
\begin{drcases}
\begin{aligned}
\dot{x} (\tau) & = f(x,\tau) + \omega \\
E[\omega(\tau)] & = 0 \\
E[\omega(\tau) \cdot \omega(\tau-t)] & = 2\Gamma \rho(\tau)
\end{aligned}
\end{drcases} \Rightarrow p(\dot{x}|x,\tau) = \mathcal{N}(f,2\Gamma)
\end{equation}
$$

Here, the random fluctuations are normally distributed with a covariance of $2\Gamma$ , under the assumption that they fluctuate sufficiently quickly, in relation to states per se, that we can ignore temporal correlations. This formulation underwrites everything that follows. In section 4, we will look more closely at where the Langevin formulation comes from – and why random fluctuations are Gaussian and uncorrelated.

**The path integral formulation**: this formulation deals with paths or trajectories $x[\tau]$, from $x(0) \equiv x0$ that are generated by the Langevin dynamics above:

$$
\begin{equation}\tag{1.2}
\begin{aligned}
\mathfrak{I}(x[\tau]) & \triangleq - \ln \space p(x[\tau]) = \mathcal{A}(x[\tau]) \\
\mathcal{A}(x[\tau]) & = \int_0^t \mathcal{L}(x,\dot{x}) d\tau \\
\mathcal{L}(x,\.{x}) & = \cfrac{1}{2}[(\.{x}-f) \cdot \cfrac{1}{2\Gamma}() + \nabla \cdot f] \\
&= \cfrac{1}{4\Gamma}\.{x}\cdot\.{x} - \cfrac{1}{2\Gamma}f\cdot\.{x} + \cfrac{1}{h}V(x) \\
V(x) & = \cfrac{h}{4\Gamma}f\cdot f + \cfrac{h}{2} \nabla \cdot f
\end{aligned}
\end{equation}
$$

This formulation expresses the probability of a path in terms of the action associated with a trajectory. It says that the surprisal (i.e., negative log probability) of a path (i.e., action) is the surprisal accumulated along its trajectory, based upon the difference between the path’s motion and the flow expected at each point in state-space. Under Gaussian assumptions about the random fluctuations, the surprisal at each point (i.e., Lagrangian) has a simple quadratic form, with an additional divergence term that arises from the implicit use of Stratonovich integrals (Seifert, 2012). See Appendix A for an explanation of this term. Here, we have expressed the Lagrangian in terms of a Schrödinger potential that will figure later in quantum mechanics. This potential depends on, and only on, the flow. For non-quantum treatments, Planck's constant is usually set to $\hbar=1$.

It will be useful to introduce the Legendre transform of the Lagrangian called a Hamiltonian that will arise in the characterisation of how things behave:

$$
\begin{equation}\tag{1.3}
\begin{aligned}
\mathcal{H}(x,\.{x}) & =\.{x}\cfrac{\partial \mathcal{L}}{\partial \.{x}}-\mathcal{L}(x.\.{x})=\.{x}\cdot p - \mathcal{L}(x,\.{x}) \\
&= \cfrac{1}{4\Gamma}\.{x}\cdot\.{x} + \cfrac{1}{h}V(x) \\
\\
p & \triangleq \cfrac{\partial \mathcal{L}}{\partial \.{x}} = \cfrac{1}{2 \Gamma}(\.{x}-f)
\end{aligned}
\end{equation}
$$


Here, the last equality defines the generalised momentum. Note that the most likely path obtains when the random fluctuations take their most likely value of zero, giving:

$$
\begin{equation}\tag{1.4}
\.{x} = f(x) \Rightarrow \mathcal{H}(x,\.{x}) = \mathcal{L}(x,\.{x}) = - \cfrac{1}{2} \nabla \cdot f(x)
\end{equation}
$$

This means that the Hamiltonian along the most likely path reduces to the divergence of the flow. Furthermore, in conservative systems with divergence-free flow (i.e., with negligible random fluctuations) the Hamiltonian is zero everywhere. This speaks to the importance of the Hamiltonian in characterising conservative (i.e., classical) mechanics. Finally, path-dependent phase measurements $\Omega (x)$ can then be averaged in the following path
integral, given an initial density, $p_0(x_0)\equiv p(x,0)$:

$$
\begin{equation}\tag{1.5}
E_{p(x[\tau],x_0)}[\Omega(x)] = \int dx_0 \int dx[\tau][\Omega(x[\tau])p(x[\tau]|x_0)p_0(x_0)]
\end{equation}
$$


This concludes the key results from the path integral formulation.

**The Fokker Planck equation**: this formulation deals with the probability density over the states, which describes the probability of finding a system in state $x$ at time $\tau$. Given a Langevin system, one can describe the density dynamics as follows:

$$
\begin{equation}\tag{1.6}
\begin{aligned}
\.{p}(x,\tau) &= Lp(x,\tau) = - \nabla \cdot j(x,\tau) \\
L &= \nabla \cdot (\Gamma \nabla - f) \\
j(x,\tau) &= f(x,\tau)p(x, \tau) - \Gamma \nabla p(x,\tau)
\end{aligned}
\end{equation}
$$

Here, $L$ is the Fokker Planck operator and $j(x,\tau)$ is the probability current that provides a convenient summary
of the flow of probability mass. This comprises a flow-dependent term and (a usually opposite) part, generated by random fluctuations over probability gradients.

#### Nonequilibrium steady states


Equipped with the Fokker Planck formulation of density dynamics, we can now consider the nonequilibrium long- term behaviour of any random dynamical system. Because the system is weakly mixing it will, after a sufficient amount of time, converge to an invariant set of states called a pullback or random global attractor. The attractor is random because it is itself a random set (Crauel, 1999; Crauel and Flandoli, 1994). The associated NESS density p(x) is the solution to the Fokker-Planck equation (Frank, 2004). Equation (1.6) shows that the NESS density depends upon flow, which can always be expressed in terms of curl and divergence-free components. This is the Helmholtz decomposition (a.k.a., the fundamental theorem of vector calculus) and can be formulated in terms of an anti-symmetric matrix $Q = −QT$ and a scalar potential $\Im(x)$ (Ao, 2004)[^note-5],

[^note-5]:For simplicity, we will assume that $Q = -QT$ does not depend on $x$, at least locally. Furthermore, the amplitude of random fluctuations is assumed to be spherical, so that we can treat $\Gamma$ as a scaled identity matrix or a scalar quantity.

$$
\begin{equation}\tag{1.7}
f =(Q-\Gamma)\nabla\Im
\end{equation}
$$

Using this standard form (Yuan et al., 2010), it is straightforward to show that $p(x) = exp(-\Im(x))$ is the solution to the Fokker Planck equation (Friston and Ao, 2012). In information theory, the scalar potential $\Im(x) = -\ln p(x)$ is known as self-information, surprisal or more simply surprise (Jones, 1979; Tribus, 1961). This means we can express the flow in terms of the NESS density or surprisal, according to the NESS lemma in Appendix B and (Friston, 2013):

$$
\begin{equation}\tag{1.8}
\begin{aligned}
f & = (\Gamma - Q)\nabla\ln p(x) \\
 & \Rightarrow \cfrac{p(x)}{j(x)} = -Q\nabla \ln p(x) \Rightarrow \.{p}(x) = 0 \\
 \space \\
\Im(x) & = - \ln \space p(x) \\
f(x) & = (Q-\Gamma)\nabla\Im(x) \\
\nabla \cdot f(x) & = - \Gamma \nabla^{2}\Im(x)
\end{aligned}
\end{equation}
$$

This is the key result upon which most of this monograph rests. It says that the flow of any random dynamical system, at nonequilibrium steady-state, comprises orthogonal components: a dissipative flow that ascends the gradients established by the logarithm of the nonequilibrium steady-state density and a conservative (divergence- free), solenoidal flow circulating on the corresponding isocontours. Heuristically, the dissipative (curl-free) flow counters the dispersion of the density that would otherwise be caused by random fluctuations. This means the only remaining probability current is solenoidal. We will see later that this simple result has some remarkable implications, when we consider the flow of various subsets of states that are conditionally independent. This particular structure rests on the notion of a Markov blanket that is the second cornerstone of all that follows.

The next move is to substitute the NESS solution to the Fokker Planck equation into the path integral formulation to express the probability of any trajectory in terms of an action, expressed in terms of surprisal. From (1.2) and (1.8) this gives:

$$
\begin{equation}\tag{1.9}
\begin{aligned}
\mathcal{A}(x[\tau]) & = \int_0^t \mathcal{L}(x,\.{x})d\tau \\
\mathcal{L}(x,\.{x}) & = \cfrac{1}{2} [ \cfrac{1}{2\Gamma}( \.{x} - Q \nabla \Im ) \cdot ( \.{x} - Q \nabla \Im) + \.{x} \cdot \nabla \Im + \Gamma(\cfrac{1}{2}\nabla \Im \cdot \nabla \Im - \nabla^{2}\Im)] \\
\mathcal{H}(x,\.{x}) & = \cfrac{1}{2} [ \cfrac{1}{2\Gamma}( \.{x} - Q \nabla \Im ) \cdot ( \.{x} - Q \nabla \Im) - \Gamma(\cfrac{1}{2}\nabla \Im \cdot \nabla \Im - \nabla^{2}\Im)] \\
\end{aligned}
\end{equation}
$$

This result uses the fact that the solenoidal and gradient flows are orthogonal $Q \nabla \Im \cdot \Gamma \nabla \Im$. Equation (1.9) is essentially the path integral formulation of nonequilibrium steady-state dynamics. It expresses the probability of any trajectory through state-space as the path integral of a Lagrangian; where the Lagrangian can be expressed in terms of motion and surprisal (i.e., the NESS potential).

Crucially, the three terms in (1.9) depend in different ways on the amplitude of random fluctuations. This dependency can be seen more clearly if we consider the expression for a one-dimensional system, where there is no solenoidal flow:

$$
\begin{equation}\tag{1.10}
\begin{aligned}
\mathcal{A}(x[\tau]) & =\underbrace{\frac{1}{2} \int_0^t \frac{1}{2 \Gamma} \dot{x}^2 d \tau}_{\text {kinetic }}+\underbrace{\frac{1}{2} \int_0^t \dot{\mathfrak{I}} d \tau}_{\text {path-independent }}+\underbrace{\frac{1}{h} \int_0^t V(x) d \tau}_{\text {path-dependent }} \\
\int_0^t \dot{\mathfrak{I}} d \tau & =\mathfrak{I}\left(x_t\right)-\mathfrak{I}\left(x_0\right) \\
V(x) & =\frac{h}{2} \Gamma\left(\frac{1}{2} \nabla \mathfrak{I} \cdot \nabla \mathfrak{I}-\nabla^2 \mathfrak{I}\right)
\end{aligned}
\end{equation}
$$


This implies that the action of any path can be expressed in terms of a motion-dependent (kinetic) term, a (path- independent) term – that depends upon the change in surprisal – and a (path-dependent) term that scales with the amplitude of random fluctuations. Appendix C provides a brief treatment of the expected Lagrangian and associated Hamiltonian.

The key thing to note here is that the first term in (1.10) has the form of a kinetic energy, in which the amplitude of random fluctuations plays the role of an inverse mass. The second term is simply a (NESS) potential difference, while the third (Schrödinger potential) term increases with the amplitude of random fluctuations. This means that when random fluctuations are large, the state behaves as if it has negligible mass and the Schrödinger potential dominates. Conversely, when the amplitude of random fluctuations is negligible, the first two terms predominate enabling a decomposition of action into kinetic and potential terms. This dialectic will appear later as the distinction between quantum and classical mechanics. Equation (1.10) suggests $\hbar = 0$ in the classical limit, when the contribution of the Schrödinger potential disappears (Feynman, 1948). However, in this monograph, Planck's constant is treated as a constant of proportionality (that endows the amplitude of random fluctuations with certain units), such that the classical limit is attained when their amplitude tends to 0; i.e., $\Gamma = 0$.

In this limit, the classical path is the most likely path that can be described with a variational principle of least action:

$$
\begin{equation}\tag{1.11}
\begin{aligned}
\delta_x\mathcal{A}(Xx[\tau]) &= 0 \\ 
&\Rightarrow \.{x}(\tau) = f(x(\tau)) \\
&\Rightarrow x[\tau] = argmin_{x[\tau]} \mathcal{A}(x[\tau])
\end{aligned}
\end{equation}
$$

This means the most likely path minimises action, rendering its variation with respect to the path zero. Crucially, at nonequilibrium steady-state, path-dependent and independent contributions to action can be expressed in terms of the surprisal and its gradients. We will call upon this consequence of nonequilibrium steady-state dynamics in several different settings. In treatments of synergetics and pattern formation, this least action principle is sometimes expressed as the destruction of energy gradients (Tschacher and Haken, 2007).

#### Fluctuations and information length

_“Time is designed in such a way that given the present, the future is independent of the past”_ (Caticha, 2015b) p6116

We will be concerned with the ‘measure’ of things; both in terms of probability measures and metrics that inherit from differential geometry. This section provides a brief background to the notion of length and information geometry – that arises when applying differential geometry to probability theory. The main message here is that all these measures depend, in a deep way, on time.

As part of this preamble, it is useful to consider the nature of random fluctuations. We will see later that these fluctuations are mixtures of states that fluctuate very quickly, in relation to states per se that play the role of slow variables. In this sense, random fluctuations are just fast states that are (by definition) not correlated with slow states. The implicit statistical independence of fast and slow states licences us to talk about ‘random’ fluctuations.

The form of the Langevin dynamics in (1.1) speaks to this separation of temporal scales. For example, the units of $\Gamma$ (per second) suggest it plays the role of a rate constant. Indeed, on one view, the amplitude of fluctuations corresponds to the rate at which the variance or dispersion of states – due to fluctuations – accumulates over time (Cox and Miller, 1965). Furthermore, at steady state, the amplitude is effectively a rate constant that couples the flow of (slow) states to the gradients of surprisal (1.7). In other words, for a given NESS density, the flow increases in proportion to the amplitude of fluctuations. One can formalise this by introducing the notion of length:


$$
\begin{equation}\tag{1.12}
\begin{aligned}
\ell = \int_0^T \sqrt{ \dot{x}(\tau)^{i} g_{ij} \.{x}(\tau)^j } dt
\end{aligned}
\end{equation}
$$

We have used the (Einstein) summation convention here, with an implicit summation over repeated superscripts and subscripts. Equation (1.12) expresses the length along a path in terms of a Riemannian metric supplied by the metric tensor $g_{ij}$. Paths of locally minimal distance are called geodesics, and are the analogues of straight lines in Euclidean space. From (1.10), the action of a path in the classical limit of low amplitude fluctuations can be interpreted as an upper bound on path length (by the Cauchy-Schwarz inequality):

$$
\begin{equation}\tag{1.13}
\begin{aligned}
 \lim_{Q,\Gamma \rightarrow 0}\mathcal{A}(x[\tau]) &= \int_0^T \dot{x}(\tau)^{i} g_{ij} \.{x}(\tau)^j dt \geq \ell^2 \\
g &= \cfrac{1}{4\Gamma}
\end{aligned}
\end{equation}
$$

For simplicity, we have ignored solenoidal flow. This suggests that the most likely (classical) path will be the shortest, if length in measured in terms of the precision (i.e., inverse covariance) of random fluctuations. Equivalently, the precision furnishes a Riemannian metric that equips state-space with a geometry in which points are close together when fluctuations have a large amplitude. The equivalence between the amplitude of random fluctuations and the metric tensor underlies our simplifying assumption that the amplitude of random fluctuations is spherical (i.e., looks the same from all directions). This is equivalent to working in a symmetric state-space, whose Riemannian metric is invariant to the choice of coordinates.

One can take this metric treatment further and equip spaces of the sufficient statistics (i.e., parameters) of a density with an information geometry. In brief, information geometry rests on Riemannian metrics that can be used to measure distances on statistical manifolds (Amari, 1998; Ay, 2015). A statistical manifold is a metric space in which each point represents a probability density; i.e., a parameter space whose points correspond to the sufficient statistics of a probability density, such that nearby points on the statistical manifold correspond to similar densities. For example, the two-dimensional space spanned by the statistical moments (i.e., mean and precision) of a Gaussian density constitutes a ubiquitous statistical manifold. The special thing about statistical manifolds is that they are always equipped with a metric tensor, supplied in the form of a Fisher information metric.

In the present setting, following (Crooks, 2007), one can characterise systemic density dynamics in terms of information length, where the metric is a Fisher information. Consider the decomposition of the density into time- independent collective variables or modes $\zeta_i(x)$ and time-dependent conjugate variables that play the role of sufficient statistics $\lambda(\tau)$ [^note-6]:

[^note-6]: We will use $Z$ to denote a partition function or normalising constant throughout.

$$
\begin{equation}\tag{1.14}
\begin{aligned}
\mathfrak{I}(x,\tau) = \lambda^i (\tau)\zeta_i (x) + \ln Z
\end{aligned}
\end{equation}
$$

이 매개변수화 하에, 피셔 정보 메트릭 $I(\lambda)$는 다음과 같습니다:

$$
\begin{equation}\tag{1.15}
\begin{aligned}
\ell & = \int_0^t \sqrt{g_{ij}\.{\lambda}^{i}\.{\lambda}^{j}} d\tau \\
g &= I(\lambda) \Leftrightarrow g_{ij} = cov(\zeta_i(x),\zeta_j(x)) = E\Bigg[\cfrac{\partial\Im}{\partial\lambda^{i}} \cfrac{\partial\Im}{\partial\lambda^{j}} \Bigg] = \cfrac{\partial D[p_{\lambda^{'}}(x)||p_{\lambda}(x)]}{\partial\lambda^{'i}\partial\lambda^{'j}}\Biggm\vert_{\lambda^{'} = \lambda}
\end{aligned}
\end{equation}
$$


Notice that the information geometry is in the space of the conjugate variables that parameterise the density over states, as opposed to state-space per se. This space is a statistical manifold and its geometry will become a central aspect of Bayesian mechanics later. At the moment it serves to foreshadow the intimate relationship between information, geometry and statistical mechanics (Crooks, 2007; Kleeman, 2014).

The final equality in (1.15) can be confirmed by straightforward calculation of the second derivative of the divergence between two probability distributions that are infinitesimally close (Caticha, 2015a); where $\lambda^{'} = \lambda + d\lambda$. This means information length on the statistical manifold accumulates more quickly when the parameterised density changes quickly. This interpretation also licences a formulation of information length as the accumulation of (the square root of) divergences between successive densities over small displacements $d\lambda \to 0$ on the statistical manifold,

$$
\begin{equation}\tag{1.16}
\begin{aligned}
\ell & = \int d \ell \\
d\ell^2 & = g_{ij}d\lambda^j d\lambda^i \\
\cfrac{1}{2}d\ell^2 &= D[p_{\lambda^{'}}(x)||p_{\lambda}(x)] = \cfrac{1}{2} \cfrac{\partial D[p_{\lambda^{'}}(x)||p_{\lambda}(x)]}{\partial\lambda^{'i} \partial\lambda^{'j}}\Biggm\vert_{\lambda^{'}=\lambda} d\lambda^j \lambda^i \\
\end{aligned}
\end{equation}
$$

The last equality follows from a Taylor expansion of the divergence, where the first non-vanishing term is the second derivative in (1.15). This follows because the divergence and its first derivative are zero when $\lambda^{'}=\lambda$ . Equation (1.16) means that information length can be construed as the number of distinct configurations the density passes through when moving through parameter space. These results provide a graceful way to connect thermodynamic variables to different configurations of a system, by treating them as parameters of a probability distribution (Crooks, 2007; Kleeman, 2014). However, our focus will be on a special parameter – time – that endows density dynamics with an information geometry.

An important information length follows from the fact that time itself parameterises an evolving density, $\lambda(\tau) = \tau \Rightarrow .{\lambda} = 1$ and therefore time has an information geometry. Consider a system prepared in some initial state with a density $p_0 \equiv p(x,0)$ such that

$$
\begin{equation}\tag{1.17}
\begin{aligned}
p(x,\tau) &= p_{0} + \tau\dot{p}_{0} + \dots \\
&= p_{0} + \tau L p_{0} + \dots \\
\\
\ell(t) &= \int_{0}^{t} \sqrt{g(\tau)}d\tau \\
g(\tau) &= I(\tau) = E_{p_{0}}[(\partial_{\tau}\Im_{0})^{2}] = \int\cfrac{(L_0 P_0)^2}{p_0}dx \\
L(\tau) &= \nabla\cdot\Gamma\nabla - \nabla\cdot f(\tau)
\end{aligned}
\end{equation}
$$

In this context, the Fisher information metric furnishes a temporal scaling that reflects the rate at which the density evolves. From (1.16):

$$
\begin{equation}\tag{1.18}
\begin{aligned}
d\ell(\tau)^2 &= g(\tau)d\tau^2 \\
\cfrac{1}{2}d\ell(\tau)^2 &= D[p(x,\tau + d\tau)||p(x,\tau)] \\
\end{aligned}
\end{equation}
$$

In other words, the metric for time plays the role of a (squared) rate constant, with units of per second (squared). Heuristically, as time progresses, information length depends upon the amplitude of random fluctuations and (the divergence of) flow via the Fokker Planck operator in (1.17). This means that metric time can proceed slowly from one part of state-space and quickly from elsewhere. Equation (1.18) also suggests that information length can be regarded as an accumulation of (squared) divergences over infinitesimally short time steps. Note that this accumulation enables a metric to be assembled from (pre-metric) divergences. This should be contrasted with the divergence between the initial density and the density at some later point in time. We will see an example of this in the next section.

The information length in (1.18) provides a useful characterisation of convergence to equilibrium or nonequilibrium steady-state (Kim, 2018). As time goes by, the future density from any initial state converges to the NESS density and the information length converges to an asymptotic limit. This limit scores the distance from the initial density to the NESS density. At convergence, the divergence in (1.18) disappears and there is no further increase in information length

$$
\begin{equation}\tag{1.19}
\begin{aligned}
\lim_{\tau \to \infty}D[p(x,\tau)||p(x)] = 0 \Rightarrow d\ell(\tau) = 0 \\
\end{aligned}
\end{equation}
$$

Effectively, from the point of view of information length, time slows down in the future. Heuristically, imagine what you will be doing in an hour – and how it differs from what you are doing at the moment. Now, repeat the exercise but imagine yourself in a decade's time and a decade plus one hour. In the sense that it is difficult to distinguish between evolving versions of yourself in the distal future, time has effectively stopped.

In summary, the information length of time-dependent densities, parameterised by time, provides a metric that complements the use of divergence between initial and final densities, which does not depend upon the path or evolution of the density from its initial state. Both play an important role in characterising convergence to nonequilibrium steady-state. Later, we will see the divergence in (1.19) arises in the form of free energy in both stochastic and Bayesian mechanics. We will also see that information length is closely related to stochastic entropy production in thermodynamic formulations. So far, everything we have previewed applies to any random dynamical system. In the next section, we will revisit these characterisations, when the system possesses a Markov blanket.

#### Random dynamical systems and Markov blankets

A Markov blanket is a set of states that separates two other sets in a statistical sense. The term Markov blanket was introduced in the context of Bayesian networks or graphs (Pearl, 1988) and refers to the children of a set (the set of states that are influenced), its parents (the set of states that influence it) and the parents of its children. The existence of a Markov blanket induces a partition of states into internal and external states, where external states are hidden (insulated) from the internal (insular) states by the Markov blanket. In other words, external states can only be seen vicariously by internal states, through blanket states. Furthermore, the Markov blanket can itself be partitioned into two sets that are, and are not, children of external states. We will refer to these as sensory states and active states respectively: $b = \lbrace s,a \rbrace \in B$ . Put simply, the existence of a Markov blanket implies a partition of states into external, sensory, active and internal states: $x = \lbrace \eta,s,a,\mu \rbrace \in X$. External states cause sensory states that influence – but are not influenced by – internal states, while internal states cause active states that influence – but are not influenced by – external states. Crucially, the dependencies induced by Markov blankets create a circular causality that is reminiscent of the action-perception cycle: see Figure 1 and (Fuster, 2004). Circular causality here means that external states cause changes in internal states, via sensory states, while the internal states couple back to the external states through active states, such that internal and external states influence each other in a vicarious and reciprocal fashion.

#### Markov blankets and marginal flows

In the next section, we will unpack the implications of Markov blankets for self-organisation in terms of information theory. This treatment rests upon the conditional independencies among the partition of states that result from precluding an influence of external states on active and internal states – and an influence of internal states on sensory and external states. This dynamical architecture is summarised in terms of a marginal flow lemma and its corollaries below. In brief, these results express the flow at nonequilibrium steady-state under the conditional independencies implied by a Markov blanket and vice versa. In other words, they connect the sparse influences mediated by Langevin flow to conditional independencies among subsets of states. Effectively, this
generalises the standard form for flow in (1.8) to a partition of states that contains a Markov Blanket. Appendix B contains the accompanying proofs and considers the complementary perspectives on how sparse influences underwrite conditional independence and vice versa.

The generalisation of the NESS density laminar to Markov blankets rests on the notion of marginal flow; namely, the flow of certain states averaged (i.e., marginalised) over other states. We will use the ~ notation to denote the complement of a subset of states; for example, $x = (\mu, \dot{\mu})$.

**Lemma** (marginal flow): for any weakly mixing random dynamical system at nonequilibrium steady-state, the marginal flow $f_{\eta}(\mu)$ of any subset of states $\eta \in X$, averaged under the complement of another $\mu \in X$ can be expressed in terms of the gradients of the logarithm of the corresponding marginal density:

$$
\begin{equation}\tag{1.20}
\begin{aligned}
f_{\eta(\mu)} \triangleq E_{p(\tilde{\mu}|\mu)}[f_{\eta}(\mu,\tilde{\mu})] = (Q_{\eta\eta}-\Gamma_{\eta\eta})\nabla_{\eta} \Im(\mu) + Q_{\eta\tilde{\eta}}\nabla_{\tilde{\eta}}\Im(\mu) \\
\end{aligned}
\end{equation}
$$

**Corollary** (conditional independence): if the flow of one subset of states does not depend on another, then it becomes the flow expected under the second subset. For example, in terms of the Markov blanket:

$$
\begin{equation}\tag{1.21}
\begin{aligned}
\begin{bmatrix}
  f_{\eta}(x) \\
  f_{s}(x)  \\
  f_{\mu}(x) \\
  f_{a}(x)  \\
\end{bmatrix} = 
\begin{bmatrix}
  f_{\eta}(\eta,x) \\
  f_{s}(\eta,x)  \\
  f_{\mu}(\mu,x) \\
  f_{a}(\mu,x)  \\
\end{bmatrix} =
\begin{bmatrix}
  (Q_{\eta\eta}-\Gamma_{\eta\eta})\nabla_{\eta}\Im(\eta,b) \\
  (Q_{ss}-\Gamma_{ss})\nabla_{s}\Im(\eta,b) + Q_{sa}\nabla_{a}\Im(\eta,b) \\
  (Q_{\mu\mu}-\Gamma_{\mu\mu\eta})\nabla_{\mu}\Im(\mu,b) \\
  (Q_{aa}-\Gamma_{aa})\nabla_{a}\Im(\eta,b) + Q_{as}\nabla_{s}\Im(\mu,b) \\
\end{bmatrix}
\end{aligned}
\end{equation}
$$

In short, the conditional independencies induced by the Markov blanket mean that the flow of external states is the same for every internal state, which is just its average over the internal states (similarly for other partitions).

**Corollary** (expected flow): the marginal flow of any subset $\eta \subset \subset x$ averaged over all other states depends only on the gradients of its marginal density, provided there is no solenoidal coupling with its complement:

$$
\begin{equation}\tag{1.22}
\begin{aligned}
f_{\eta}(\eta) = (\Gamma_{\eta\eta} - Q_{\eta\eta})\nabla_{\eta}\ln p(\eta) = (Q_{\eta\eta} - \Gamma_{\eta\eta})\nabla_{\eta}\Im(\eta) \\
\end{aligned}
\end{equation}
$$

This is a special case of the marginal flow lemma, when $\eta = \mu$ and $Q_{\eta\eta}=0$ . It implies that the expected flow of any state or subset of states, averaged over all other states, will behave in exactly the same way as all states considered together. In other words, it will ascend the gradients of its (marginal) density.

The marginal flow lemma allows us to express the conditional independencies implicit in the structural or probabilistic graphical model of Figure 1 in terms of the flows in (21). In other words, if a system maintains a Markov blanket at nonequilibrium steady-state, then it must possess flows that depend only upon certain states. This structured dynamics underwrites everything that follows.

#### Summary

This section has introduced the technical foundations that we will call upon later to characterise dynamics in various settings. Its focus was on self-organisation to nonequilibrium steady-state, which can be characterised as the solution to the Fokker Planck formulation of density dynamics. Crucially, this enables one to express the flow of states in terms of a nonequilibrium steady-state density, surprisal or potential. We have looked briefly at the geometry of density dynamics in terms of information length. Finally, the conditional independencies implied by a Markov blanket have been expressed in terms of how the (marginal) flow of certain states depends on other states. The marginal flows induced by a Markov blanket will become important later, when we interpret gradient flows in relation to information geometry – in Part Three.

[Figure 1](./img/01.png)
<p style="text-align: center;">FIGURE 1</p>

_Markov blankets_. This probabilistic graphical model illustrates the partition of states into internal states (blue) and hidden or external states (cyan) that are separated by a Markov blanket – comprising sensory (magenta) and active states (red). The upper panel shows this partition as it would be applied to action and perception in a brain. In this setting, self-organisation of internal states then corresponds to perception, while active states couple brain states back to external states. The lower panel shows the same dependencies but rearranged so that the internal states are associated with the intracellular states of a Bacillus, where the sensory states become the surface states or cell membrane overlying active states (e.g., the actin filaments of the cytoskeleton). Note that the only missing influences are between internal and external states – and directed influences from external (respectively internal) to active (respectively sensory) states. The surviving directed influences are highlighted with dotted connectors. Autonomous states are those states that are not influenced by external states, while particular states constitute a particle; namely, autonomous and sensory states – or blanket and internal states. The equations of motion in the upper panel follow from the marginal flow lemma.

### Symmetry breaking and self-organsation

_"How can the events in space and time which take place within the spatial boundary of a living organism be accounted for by physics and chemistry?"_(Schrödinger, 1944)

The introduction of Markov blankets – and the distinction between the external and internal states of a particle – changes the game somewhat, in terms of ensemble densities. In the absence of a partition, we can only talk about the entropy of a density and how it changes with time. However, in the setting of a partition, we can consider the entropy of particular states in relation to hidden states (or vice versa). This relative entropy is known as mutual information. So, are we interested in systems with a high or a low mutual information? It transpires that the answer is both, in the sense that we are interested in particles that explore their state-space but have a well-defined attracting manifold with low measure (i.e., low entropy). This speaks to a dialectic between opposing constraints. In brief, if the NESS entropy of particular states is small, then the average uncertainty about particular states, given external states must be small. In other words, knowing the external state resolves ambiguity about particular states. However, at the same time, the mutual information or coupling between external and particular states must also be small; otherwise, there will be a risk of being unable to disambiguate external from particular states; i.e., the particle will dissipate or dissolve. Heuristically, this allows for the fact that we can identify Markov blankets that are distinct from their external milieu (e.g., disambiguating a fish from the water in which it is swimming), while – at the same time – observing an intricate and self-organised coupling between particular dynamics and external states (e.g., a particular fish swimming in water). Even more simply, a fish remains a fish, despite the myriad of delicate, context-sensitive behaviours that preserve its integrity (Clarke et al., 2015). In what follows, we consider how this dialectic emerges from a straightforward statistical treatment using information theory.

Having established a partition of systemic states, we are now in a position to define the sort of self-organising systems we want to characterise. In brief, these are systems with space-filling random dynamical attractors with low measure. In other words, their probability mass is concentrated in small volumes that are connected in a way that permits itinerant (i.e. wandering) percolation of trajectories through state-space, from one manifold of the attractor to another: c.f., the percolation produced by phase transitions in deterministic systems (Vespignani and Zapperi, 1998). The implicit symmetry breaking (i.e., divergence of nearby trajectories to different regimes of phase-space) is a hallmark of nonequilibrium dynamics (Evans and Searles, 2002) and is intimately related to phenomena like self-organised criticality in dynamical systems (Bak et al., 1988; Vespignani and Zapperi, 1998). Indeed, much of complexity science addresses the problem of how to formalise multiscale, itinerant and chaotic dynamics. This is a vast field, encompassing renormalisation group theory, scale-invariance, criticality and universality (Kwapien and Drozdz, 2012; Nicolis and Prigogine, 1977; Schwabl, 2002). In this monograph, we will elude many of the finer details (and phenomena such as bifurcations, frustration and phase transitions) and suppose that the interesting behaviour of self-organising systems can be captured by nonequilibrium steady-state densities with the right sort of shape.

So, what is the right sort of shape? We start by considering the marginal (NESS) density over particular states. Given a partition into external and particular states, it is straightforward to characterise a simple form of self-organisation in terms of entropy production. This follows because there is a separation between autonomous $\alpha =\lbrace a,\mu\rbrace \in A$ and sensory states $s \in S$. Crucially, by definition, the flow of autonomous states does not depend on external states $\eta \in E$. This means that autonomous states will appear to suppress the self-information or surprisal of particular states $\pi\in P$ and its long-term average; namely, their entropy. From the marginal flow lemma (1.21), we have (ignoring solenoidal coupling between active and sensory states):

$$
\begin{equation} \tag{2.1}
\begin{aligned}
f_{\alpha}(\pi) &= (Q_{\alpha\alpha} -\Gamma_{\alpha\alpha})\nabla_{\alpha}\Im(\pi) \\
E_{p(\pi)}[\Im(\pi)] &= lim_{\tau\to\infty}\frac{1}{\tau}\int_{0}^{\tau}\Im(\pi(t))dt \\
&= H(P)
\end{aligned}
\end{equation}
$$

We will refer to the entropy of particular states as particular or self-entropy. The flow in (2.2) will make it look as if autonomous states are trying, on average, to minimise the entropy of particular states. From elementary information theory, it follows that autonomous states will also look as if they are trying to minimise the mutual information between external states and particular states, while – at the same time – minimising the entropy of particular states, given external states. This is because mutual information is the uncertainty about particular states, minus the uncertainty, given external states (i.e., when there is no reduction in uncertainty afforded by knowing the external states, the mutual information is zero).

The decomposition of (self) entropy into mutual information and conditional entropy can also be expressed, from a statistical perspective, as a decomposition of surprisal into inaccuracy and complexity:

$$
\begin{equation} \tag{2.3}
\begin{aligned}
\Im(\pi) &= E_{p(\eta|\pi)}[\Im(\pi)] \\
&= E_{p(\eta|\pi)}[\ln p(\eta|\pi) - \ln p(\pi|\eta)] \\
&= E_{p(\eta|\pi)}[\ln p(\eta|\pi) - \ln p(\eta) - \ln p(\pi|\eta)] \\
&= \underbrace{E_{p(\eta|b)}[\Im(\pi|\eta)]}_{\text{inaccuracy}} + \underbrace{D[p(\eta|\pi)||p(\eta)]}_{\text{complexity}} \\
\\
E_{p(\pi)}[\Im(\pi)] &= \underbrace{H(P)}_{\text{entropy}} = \underbrace{H(P|E)}_{\text{ambiguity}} + \underbrace{I(E,P)}_{\text{risk}} \\
\underbrace{H(P|E)}_{\text{ambiguity}} &= \underbrace{H(P)}_{\text{entropy}} - \underbrace{I(E,P)}_{\text{info gain}} \\
\end{aligned}
\end{equation}
$$

Complexity here is used in a statistical sense, where it scores the divergence between a posterior and prior distribution over external (hidden) states, while accuracy is the expected log probability of particular states, under the posterior. On this view, the conditional entropy is expected inaccuracy (i.e., ambiguity), while mutual information becomes the expected complexity cost (i.e., risk). The last equality evinces the dialectic that attends mutual information: on the one hand, minimising entropy requires the minimisation of mutual information, where it plays the role of risk, while minimising ambiguity requires a maximisation of mutual information, where it plays the role of information gain. These complementary roles are easily reconciled by noting that ambiguity and risk (or inaccuracy and complexity) are just two sides of the same coin; namely, self-entropy.

Complexity is a ubiquitous cost function in optimal control theory and Bayesian statistics. In optimal control, it scores the divergence between predicted external states, given the sensory and active (control) states and some desired states (Kappen, 2005; Kappen et al., 2012). In economics, this is called risk-sensitive control (Fleming and Sheu, 2002; van den Broek et al., 2010). In Bayesian statistics, the complexity scores the degree to which a posterior density over hidden states diverges from its prior; in other words, the degrees of freedom required to encode posterior beliefs about hidden states (Spiegelhalter et al., 2002). Reducing complexity cost underwrites Occam's principle; i.e., the best explanation provides an accurate account with the smallest change in posterior beliefs relative to prior beliefs (Penny et al., 2004). Formally, this is closely related to the notion of causal entropic forces in the modelling of adaptive behaviour in nonequilibrium systems (Wissner-Gross and Freer, 2013). Finally, the causal entropic forces can, themselves, be related to the maximum entropy principle of Jaynes (Jaynes, 1957). 

The ambiguity term has epistemic, uncertainty reducing, interpretations; in which the marginal flow of autonomous states will appear to minimise the uncertainty about sensory states, given external states. In other words, self-organisation will appear to seek out regimes of phase-space in which external states cause unambiguous sensory states – much like searching under a lamp post for lost keys (Demirdjian et al., 2005). This dynamics is self-organising in the sense that (on average) autonomous states will appear to reduce the entropy of particular states. This particular entropy is the mutual information between blanket and external states plus their conditional uncertainty, conditioned on the external states. In other words, autonomous states will appear to minimise the statistical coupling (i.e., mutual information) with external states while, at the same time, resisting their dispersion, under any given hidden states.

We can express this active resistance to dissipation in terms of entropy production (a full treatment of entropy production can be found in the thermodynamics section below). The entropy production due to the flow of autonomous states can be expressed as:

$$
\begin{equation} \tag{2.4}
\begin{aligned}
\dot{H}^{\alpha} &= \int p(\pi) f_{\alpha}(\pi)\cdot\nabla_{\alpha}\Im(\pi)d\pi \\
&= -\int p(\pi)\nabla_{\alpha} \Im(\pi)\cdot\Gamma_{\alpha\alpha}\nabla_{\alpha}\Im(\pi)d\pi \leq 0
\end{aligned}
\end{equation}
$$

It follows that autonomous entropy production is always zero or less (because the covariance of random fluctuations is positive definite – and the solenoidal flow cancels). In other words, at nonequilibrium steady-state, autonomous flow resists the dispersion of particular states due to random fluctuations and the influences of external states. We can drill down on this entropy reducing behaviour by considering the marginal flow of autonomous states expected under sensory states. By the marginal flow lemma (1.22), we have:

$$
\begin{equation} \tag{2.5}
\begin{aligned}
f_{\alpha}(\alpha) = (Q_{\alpha\alpha} - \Gamma_{\alpha\alpha})\nabla_{\alpha}\Im(\alpha) \Rightarrow p(\dot{\alpha}|\alpha) = \mathcal{N}(f_{\alpha}(\alpha), 2\Gamma_{\alpha}) \\
\end{aligned}
\end{equation}
$$

Following (1.11), when random fluctuations dominate, the most likely (marginal) path of autonomous states minimises their action:

$$
\begin{equation} \tag{2.6}
\begin{aligned}
\delta_{\alpha}\mathcal{A}(\alpha[\tau]) &= 0 \\
&\Rightarrow \dot{\alpha} = f_{\alpha}(\alpha) = (Q_{\alpha\alpha}-\Gamma_{\alpha\alpha})\nabla_{\alpha}\Im (\alpha) \\
&\Rightarrow \alpha[\tau] = argmin_{\alpha[\tau]}\mathcal{A}(\alpha[\tau]) \\
\end{aligned}
\end{equation}
$$

So, what does this entail? To build an intuition about autonomous dynamics, we can use the same inflationary device as in (2.3) to express the surprisal of autonomous states in terms of complexity cost and the information gained by conditioning on sensory states:

$$
\begin{equation} \tag{2.7}
\begin{aligned}
\Im(\alpha) &= E_{p(\tilde{\alpha}|\alpha)}[\Im(\alpha)] \\
&= E_{p(\tilde{\alpha}|\alpha)}[\ln{p(\eta|\pi)} - \ln{p(\eta)} - \ln{p(\eta|\pi)} + \ln{p(\eta|\alpha)} - \ln{p(\alpha|\eta)}] \\
&= E_{p(\eta|\alpha)}[\Im(\alpha|\eta)] + E_{p(\tilde{\alpha}|\alpha)}[\underbrace{D[p(\eta|\pi)||p(\eta)]}_{\text{complexity}} - \underbrace{D[p(\eta|\pi)||p(\eta|\alpha)]}_{\text{information gain}}] \\
E_{p(\tilde{\alpha}|\alpha)}[\Im(\alpha)] &= H(A) = I(A,E) + H(A|E) \\
&= H(A|E) + \underbrace{I(E,P)}_{\text{risk}} - \underbrace{I(E,S|A)}_{\text{active information}} \\
\end{aligned}
\end{equation}
$$

Here, $\tilde{\alpha} =\{\eta,s\}$ is the complement of autonomous states. This decomposition means that the marginal flow of
autonomous states minimises its surprisal, which can be decomposed into terms that reflect the dialectic between trying to couple to external states and yet resist their dispersive effects. In this decomposition, ambiguity reduction is expressed in terms of information gain:

$$
\begin{equation} \tag{2.8}
\begin{aligned}
\underbrace{E_{p(\pi)}[D[p(\eta|\pi)||p(\eta|\alpha)]]}_{\text{expected information gain}} = I(E,S|A) = I(E,S) - I(E,S,A) \\
\end{aligned}
\end{equation}
$$

This equality has been introduced to establish a connection with characterisations of self-organisation in terms of higher-order mutual information below. Information gain is sometimes referred to as epistemic value or intrinsic motivation in artificial intelligence and robotics (Friston et al., 2015b; Oudeyer and Kaplan, 2007; Schmidhuber, 2010). It corresponds to change in the probability density over external states afforded by sensory states: i.e., the Kullback-Leibler (KL) divergence between the posterior density with and without sensory states, conditioned upon autonomous states. This is also the mutual information between the sensory and hidden states, afforded by autonomous activity. In the life sciences (e.g., cognitive neuroscience), this measure is often referred to as Bayesian surprise or salience (Itti and Baldi, 2009; Mirza et al., 2016; Sun et al., 2011). We will return to these interpretations in Part Three. The expression for expected information gain in (2.8) shows that it comprises the mutual information between external and sensory states minus the third order mutual information (among external, sensory and autonomous states).

In summary, self-organisation can be cast as an autonomous suppression of self-entropy (resp. surprisal). In turn, self-entropy can be decomposed into risk (resp. complexity) and ambiguity (resp. inaccuracy) resolving components that look as if they are mediated by the flow of autonomous states. Clearly, in one sense, all interesting systems that possess a random dynamical attractor will show some degree of self-organisation. Expressing self- organisation in terms of self-entropy, risk and ambiguity just means that one can talk about – and quantify – self- organisation in terms of sentient, epistemic behaviour.

#### Self-organisation and self-evidencing

In statistics, the surprisal of particular states is known as the negative logarithm of the marginal likelihood or evidence. This means self-organisation can be construed as self-evidencing, in the sense that the most likely flow of autonomous states reduces surprisal and therefore increases evidence. This interpretation will play an important role in Part Three, in terms of understanding behaviour – of the sort considered in computational and cognitive neuroscience. The position taken here is not to ask how self-organisation emerges; rather, what properties do self- organising systems exhibit? This may seem as if we are avoiding a hard problem; however, nearly every system encountered in the real world is self-organising to a greater or lesser degree – suggesting that self-organisation is, in itself, unremarkable. Put another way, if systems did not self-organise they would have dissipated before we had a chance to observe them. This means that the interesting questions are what self-organisation looks like and what sort of mechanics does it entail?

In what follows, we look at how self-organisation is manifest and, in Part Three, turn to the apparent teleology that emerges from a Bayesian mechanics. From the point of view of a physicist, this means we are starting from the assumption that any interesting system that has a random dynamical attractor will, in the course of settling onto its attracting set, reduce its entropy. This stands in stark contrast with statistical thermodynamics that normally appeals to an increase in the entropy of a closed system. However, the very closure of the system – in terms of its insulation from external states by a Markov blanket – may be the more interesting problem. In other words, how did the heat bath or container emerge and what explains its persistence? This is not to say that classical (and equilibrium) statistical mechanics go away: we will see in subsequent sections how they emerge as special cases, when we consider ensembles of Markov blankets contained within blankets.

#### Self-organisation, frustration and supersymmetry

The preceding characterisation of self-organisation was introduced heuristically; however, it has some construct validity in relation to various characterisations of complexity. Perhaps the most direct is the relationship between high-order mutual information and the itinerant dynamics associated with (geometrical) frustration in dynamical systems (Kaluza and Meyer-Ortmanns, 2010). In particular, the correlations among ensembles with negative third-order mutual information can be considered frustrated, in the sense that “two-body preferences are simultaneously unsatisfied” (Matsuda, 2000) p3099. These correlations are especially important in frustrated statistical systems such as spin glasses. In these systems, frustration – due to competing interactions or geometrical constraints – can induce complicated phase transitions, partial disorder, and non-exponential relaxation (Fierro et al., 1999; Matsuda, 2000). Interestingly, high-order mutual information also underpins the measures of neural complexity introduced by (Tononi et al., 1994): see (Ay, 2015).

The current formulation (in terms of random dynamical systems) is probably best considered in relation to the supersymmetry theory of stochastic systems (Parisi and Sourlas, 1982). All stochastic differential equations for continuous time dynamical systems – of the sort we are dealing with here – possess topological supersymmetry (Ovchinnikov, 2016). Topological supersymmetry (TS) refers to the preservation of phase-space continuity; in other words, infinitely close points remain close during continuous time evolution, even in the presence of noise. Spontaneous TS breaking underpins ubiquitous dynamical phenomenon; such as chaos, turbulence and self- organized criticality (Ovchinnikov, 2016). Symmetry breaking of this sort entails the emergence of long-range dynamical behaviour by the Goldstone theorem (Goldstone et al., 1962). This manifests as 1/f noise and the scale- free statistics of sudden (instantonic) processes that conform to Zipf's law; e.g., earthquakes, neuronal avalanches, solar flare etc., (Beggs and Plenz, 2003; Kauffman and Johnsen, 1991; Newman, 2005; Plenz and Thiagarajan, 2007; Shew et al., 2011).

To explain this kind of dynamical behaviour, it has been suggested that some random dynamical systems are attracted to critical points. This constitutes the phenomenological approach of self-organized criticality – SOC (Bak et al., 1987; Bak et al., 1988). Spontaneous TS breaking offers an alternative perspective that eschews critical phenomena and regards SOC as noise-induced symmetry breaking. Heuristically, this can be thought of as noise- induced tunnelling among different attracting manifolds. Figure 2 helps build an intuition about symmetry breaking by illustrating its emergence as self-entropy is reduced. A complementary illustration is provided in Figure 3, which shows the emergence of dynamical instability (i.e., criticality) as self-entropy falls.

[Figure 2](./img/02.png)
<p style="text-align: center;">FIGURE 2 </p>

Self-evidencing, self-organisation and scale-free dynamics. This figure illustrates the itinerant, scale-free dynamics that emerge with the reduction of self-entropy – and the mutual information between external and blanket states. This simple example starts with a fixed-form likelihood (upper left panel) mapping from external or hidden states to a particle’s states. For simplicity, there are no internal states in this simulation, so the particle is constituted by blanket states. Here, one hidden state maps to a blanket state via a nonlinear (quadratic) function with a state-dependent dispersion (modelled with a quadratic function of the hidden state). The self-entropy was minimised with respect to the marginal density over hidden states (using a gradient descent). The ensuing joint distributions are shown in the middle row, as mutual information decreases over iterations of the gradient descent. The black and red lines correspond to the marginal densities over hidden and blanket states, respectively. The key observation here is that the joint distribution progressively concentrates probability mass in regions that reduce mutual information, while avoiding regions with a high conditional uncertainty over sensory states. This is reflected in the mutual information measures shown in the upper right panel. In this example, decreases in self-entropy entail a decrease in mutual information (i.e., expected complexity or risk), with slight increases in conditional uncertainty (i.e., ambiguity). Given the joint distribution, one can derive the flow and solve for particular trajectories (here, over 220 time steps). The lower left panel shows the flow in terms of a quiver plot and part of the trajectory (over 210 time steps, assuming the amplitude of random fluctuations was unity with solenoidal flow of one quarter). This segment was chosen to illustrate noise-induced tunnelling; i.e., a trajectory that connects the two regimes of the attracting set. Technically, this is known as an instanton (Ginzburg, 1987). The associated dynamics show itinerancy as the trajectory wanders within the attracting set. The ensuing scale-free behaviour is illustrated in the lower right panel in terms of a power law. Here, the log spectral density has been plotted against log frequency; showing a roughly linear relationship with a power law exponent of -1.42. Technically, this corresponds to a noised induced (N–phase) breaking of topological supersymmetry or, more colloquially, noise induced tunnelling from one regime of the attracting set to another. Although this scale-free dynamics resembles anomalous diffusion – usually associated with non-extensive (or non-Gaussian) dynamics; e.g., (Pavlos et al., 2012) – it emerges from extensive (Gaussian) dynamics, under a joint density that was optimised to induce self-organising flow. The cyan and magenta dots correspond to the equivalent simulation at earlier iterations, to illustrate the emergence of power law scaling. These simulations used a discretised state-space of 128 bins for each of the two states. The trajectory was integrated using a simple Euler scheme.

[Figure 3](./img/03.png)
<p style="text-align: center;">FIGURE 3 </p>

Symmetry breaking and bifurcations. This figure illustrates the relationship between particular (i.e., self) entropy and the exponential divergence of trajectories that underlies symmetry breaking in the (stochastic) Lorentz system (Agarwal and Wettlaufer, 2016; Lorenz, 1963). This example illustrates how entropy changes with bifurcations and their associated (random) attracting sets. Here, we integrated a Lorenz system (for $2^{18}$ time steps of 1/64 units of time) with increasing values of the Rayleigh (control) parameter that, in deterministic systems, induces a pitchfork bifurcation (at $\rho$ = 1) and a subsequent (subcritical) Hopf bifurcation (at $\rho$ = 24.74). Because we added small (standard deviation of 1/128) random fluctuations to the flow, noise induced topological symmetry breaking emerges around $\rho$ = 14 (typically, in a regime of chaotic transients). The exponential divergence of trajectories was measured with the maximal Lyapunov exponent (averaged over the orbits). The resulting changes in the Lyapunov exponent (right panel) cause the attracting set to become space-filling (see insets beneath), with associated changes in self-entropy and mutual information (left panel). Here, we exploited the fact that the flow of the Lorenz system has one missing link (from the third to the first state). This means we can associate the first state with an active state, the second with a sensory state and the last with an external or hidden state (note there are no internal states here and the particular states reduce to blanket states). The remarkable result in this simulation is that the highest degree of self-organisation – as reflected in the entropy of the (active and sensory) blanket states shows a profound dip just before the onset of stochastic chaos – in a regime associated with critical slowing in deterministic systems. The insets illustrate the bifurcations and attracting sets, in terms of illustrative trajectories (right) and associated ensemble densities (left), arbitrarily rescaled to the minimum and maximum values of the trajectory. Cardinal bifurcations are illustrated with vertical lines, while the horizontal line indicates when the principal Lyapunov exponent first crosses zero at the onset of (stochastic) chaos. The mutual information measures (between the first and remaining states) were evaluated using a discretisation of state-space into 32 bins in each of the three dimensions. This example is offered as a numerical study to illustrate that a simple definition of self-organisation – in terms of the entropy of blanket (i.e., particular) states – has some construct validity in relation to self-organised criticality in stochastic chaos: a validation that may or may not generalise. Note that the dynamics illustrated here are not deterministic because each state is equipped with random fluctuations. We will see later that this means each state of the Lorenz attractor is modelled as a mixture of blanket states at lower scale – that inherit fast fluctuations from their internal states.

#### Self-organisation and information length

So far, we have considered self-organisation in terms of particular entropy, where a low entropy appears to go hand-in-hand with the phenomenology of symmetry breaking and self-organised criticality. This begs the question: how can one quantify itinerancy of this sort? One approach borrows the notion of information length; namely, the number of discernible probabilistic configurations a system passes through en route to nonequilibrium steady-state. In other words, one can associate itinerant symmetry breaking (of the sort seen in biological systems) with long information lengths from a particular state to nonequilibrium steady-state. The use of information length eludes difficult questions about the meaning of high versus low self-entropy, which is only defined to within an additive constant (Jones, 1979). Conversely, the information length is a metric that can be applied to any density dynamics to score the wandering, itinerant dynamics we are trying to quantify.

To build an intuition about information length, Figure 4 shows three examples that illustrate the role of flows and random fluctuations in generating itinerant but structured dynamics. In this illustration, we use the Lorentz system of Figure 3 to show the different ways in which an initial density – given a particular state – converges to the nonequilibrium steady-state density. The upper panel shows the familiar self-organisation induced by the Lorentz attractor, using low amplitude random fluctuations. In this regime, the system has undergone a Hopf bifurcation, guaranteed by using a Rayleigh parameter of 28. The evolution of the initial density was evaluated in terms of: (i) its KL divergence from the NESSdensity $D(\tau)$ –and(ii)the difference in information length between the density over time and the final (steady-state) density $\Delta(\tau)$.

$$
\begin{equation} \tag{2.9}
\begin{aligned}
D(\tau) &= D[p(x,\tau|\pi_0) \parallel p(x,\infty|\pi_0)] \\
\delta(\tau)^2 &\leq \frac{1}{2}D(\tau) \\
\\
\Delta\ell(\tau) &= \ell(\tau) - \ell(\infty) \\
\frac{1}{2}d\ell(\tau)^2 &= D[p(x,\tau+d\tau|\pi_0) \parallel p(x,\tau|\pi_0)] \\
\\
D(\tau) &= 0 \Leftrightarrow \Delta\ell(\tau) = 0 \Leftrightarrow \delta(\tau)=0 \Leftrightarrow d\ell(\tau)  = 0 \\
\end{aligned}
\end{equation}
$$

The inequality above is known as Pinsker's inequality, where, $\delta(\tau)$ is called total variation distance (Rényi, 2007) and is upper bounded by $D(\tau)$ , which we will refer to as divergence length. Recall from (1.18) that the  characterisations of statistical distances $D(\tau)$ and $\Delta(\tau)$
are related but differ in their use of KL divergences. The path length is an accumulation of divergences over small increments over time – to ensure the information length is a (Riemannian) measure of distance. Conversely, the divergence length between initial and final densities is not. The final expression in (2.9) says that after a sufficient period of time the density ‘forgets’ about the particular state it started from; rendering increments in divergence and information length zero. Conversely, particles that ‘remember’ their initial state have a long information length with itinerant density dynamics.


A long information length means, effectively, the initial density is a long way away from the final density and therefore convergence takes longer (indicated by the small blue arrows in Figure 4). In this example, it takes about eight seconds before convergence to steady state. This can be contrasted with the lower panels that illustrate examples of fast convergence; meaning that the initial densities have a short information length.

As one might intuit from inspection of (1.1), there are two ways to reduce information length. First, one can increase the amplitude of random fluctuations while keeping the flow fixed. This enables trajectories to explore state-space quickly and find their attracting set from any initial density. Panel B illustrates this by increasing the amplitude of random fluctuations – by decreasing their log precision from 8 to 0. This markedly attenuates information length, such that convergence to nonequilibrium steady-state takes less than a second. Alternatively, one can change the flow, without changing the amplitude of random fluctuations. The example in panel C features the same reduction of information length – and accompanying KL divergence – when the Rayleigh parameter was reduced from 28 to 1. In this flow regime, the Lorentz attractor becomes a point attractor and the itinerancy due to stochastic chaos is lost (see Figure 3).

Generally speaking, the information length preserves the linearity of the system’s dynamics. For example, with linear flow we have a familiar Ornstein–Uhlenbeck process, where information length decreases with the amplitude of random fluctuations. Following (Kim, 2018):

$$
\begin{equation} \tag{2.10}
\begin{aligned}
f(\pi) &= -\gamma\pi + \omega \\
&\Rightarrow \ln{\ell(\infty)}=\ln{|\pi_0|} + \tfrac{1}{2}\ln{\gamma} - \tfrac{1}{2}\ln{\Gamma} \\
&\Rightarrow \frac{\partial\ln\ell(\infty)}{\partial\ln{|\pi_0|}} = v = 1
\end{aligned}
\end{equation}
$$

In contrast, nonlinear flow changes the linear scaling of geometric structure to produce power-law scaling $v \ne 1$ characteristic of symmetry breaking, itinerancy and self-organised criticality[^note-7]. An interesting aspect of the numerical analyses of chaotic systems in (Kim, 2018) is the dependency of information length on the initial state, where unstable or critical points have the shortest information length. From the numerical analysis in Figure 3, one might picture noise-induced tunnelling from unstable points as mediating ‘shortcuts’ to nonequilibrium steady-state. The linear case suggests that as random fluctuations attain large amplitudes, all initial conditions are drawn close to steady-state and, by implication, self-organisation to nonequilibrium steady-state is (almost) instantaneous (c.f., Panel B of Figure 4). Later, we will associate this sort of behaviour with small (quantum) particles.

[^note-7]: See Kim, E.-j., 2018. Investigating Information Geometry in Classical and Quantum Systems through Information Length. Entropy 20, 574. for further discussion and an (entertaining) application of information length to music.

In Part Three, we will look more closely at self-organisation in systems that have a long information length – and contrast these particles with short information length systems, such as quantum and other small particles (e.g., viruses). On this view, information length distinguishes between the simple, fast, ‘hot’ self-organisation of small (quantum) particles and the itinerant, slow, ‘cold’ behaviour of large (classical) particles.

[Figure 4](./img/04.png)
<p style="text-align: center;">FIGURE 4 </p>

Convergence to nonequilibrium steady-state. A: this is a simple demonstration of (nearly) deterministic convergence to nonequilibrium steady-state, using the Lorenz system of Figure 3. Deterministic solutions (with a Rayleigh parameter of 28) were obtained for 8192 initial states, integrating over eight seconds (with a time step of 1/64 seconds and low amplitude random fluctuations with a log precision of eight). The initial particular states were the same for each solution and yet their final density converges to non-equilibrium steady-state over time. This manifests as a collapse in the divergence between the sample densities and final (NESS) density – as evaluated using a Gaussian approximation to the ensemble densities at each point in time. The upper insets show the propagated sample densities at four points in time. As time progresses, this density comes to assume the familiar butterfly form of the Lorenz attractor. However, these solutions are not trajectories through state- space, they are the endpoints of paths from an ensemble of starting locations (shown in the right plot). For comparison, convergence is also shown in terms of relative information length. One can see that information length effectively stops increasing when the divergence is zero. The lower panels show the same simulations but using random fluctuations with a log precision of zero (i.e., a variance of one) – panel B – and a Rayleigh parameter of one – panel C. In these illustrations, we treated the first state of the Lorenz system as the active state, the second state constituted the sensory state and the third state played the role of an external or hidden state. This designation is based upon the fact that the first state is not influenced by the third. This numerical example shows how uncertainty about external states is propagated over time to induce uncertainty about a particle’s state; even when the initial (particular) state is known.

#### Summary

The treatment in this section suggests that self-organising systems reduce their self-entropy, to the extent allowed by coupling to external states (or other Markov blankets) and random fluctuations. Using information theory, it is possible to interpret this kind of behaviour in terms of statistical imperatives; namely, the avoidance of complexity cost (i.e., risk) and inaccuracy (i.e., ambiguity). The Nirvana of simple self-organisation is a complete resolution of particular or self-entropy: a trivial solution here would be when a particular density collapses to a point mass (i.e., a delta function). Although we are not interested in these simple solutions, it is interesting to reflect that small particles may be trying to get back to how the universe started. A more interesting example of itinerant self- organisation is provided in Figure 4. In Part Three, we will return to the emergence of self-organisation and symmetry breaking. In brief, we will see that systems with these characteristics can always be construed as engaging in something called active inference (a.k.a. self-evidencing) via a minimisation of a variational free energy.

Table 1 provides a summary of the information measures introduced in the section, which we will refer to later. However, before dealing with the sentient foundations of self-organisation, we will spend some time unpacking the NESS lemma (Appendix B) in terms of Markov blankets (in the remainder of Part One) and its relationship to quantum, statistical and classical mechanics (in Part Two) – to contextualise later treatments of active inference (in Part Three)

[Table 1](./img/t1.png)

### Synthetic soups and active matter

In this section, we describe an exemplar system that will be used to illustrate crosscutting themes in subsequent sections. Here, it is used to simulate a primordial soup – to illustrate the emergence of self-organisation in terms of Markov blankets and internal states. This soup or active matter (Ramaswamy, 2010), comprises an ensemble of particles that are coupled through short range interactions. Each particle corresponds to the Lorentz system of the previous section that has been ‘dressed’ with blanket states to create an internal state – and enable interactions among particles. The resulting simulations are similar to those used to characterise pattern formation in dissipative systems; for example, Turing instabilities (Turing, 1952) and other dissipative structures in nonequilibrium systems, such as turbulence and convention in fluid dynamics (e.g., Bénard cells) or percolation in reaction-diffusion systems such as the Belousov-Zhabotinsky reaction (Belousov, 1959). In our case, we can treat our system is an ensemble of macromolecules; however, the details of the simulation are not important, similar results would be obtained with any coupled random dynamical system. The description below summarises the material in (Friston, 2013), where interested readers can find more details.

#### An active soup

To simulate the emergence of a Markov blanket, each constituent of the ensemble or i-th macromolecule was
equipped with notional Newtonian and electrochemical states, $\{b_n^{(i)} , b_e^{(i)}\}$. Here, $b_n^{(i)}=\{a_n^{(i)} , s_n^{(i)}\}$ can be considered coordinates of motion; e.g., position and velocity, while $b_e^{(i)} = \{a_e^{(i)} , s_e^{(i)},\mu^{(i)} \}$ could correspond to electrochemical states; e.g., oncentrations or electromagnetic states. The electrochemical dynamics of each macromolecule was chosen to have a Lorenz attractor, which provides a ubiquitous model of itinerant systems; e.g. in electrodynamics, lasers and chemical reactions (Poland, 1993). Figure 5 provides the summary of the dynamics. Specifically, the Langevin equation for the $i$-th macromolecule is:

$$
\begin{equation}\tag{3.1}
\begin{aligned}
\begin{bmatrix}
  \dot{s}_e^{(i)} \\
  \dot{a}_e^{(i)}  \\
  \dot{\mu}^{(i)} \\
\end{bmatrix} &= 
\begin{bmatrix}
  10(a_e^{(i)}-s_e^{(i)})+s_e^{(i)}) \\
  32\cdot s_e^{(i)} -a_e^{(i)} -\mu^{(i)} s_e^{(i)} \\
  s_e^{(i)}a_e^{(i)} - \tfrac{8}{3}\mu^{(i)} \\
\end{bmatrix} \cdot K^{(i)} + \omega_e \\
\\
s_e^{(i)} &= \textstyle\sum_{j=\{j:\Delta_{ij}<1\}}s_e^{(i)} \\
\Delta_{ij} &= |a_n^{(j)} - a_n^{(i)}|
\end{aligned}
\end{equation}
$$

Here, changes in electrochemical states are coupled through the local average $s_e^{(i)}$ of the states of other macromolecules that lie within a distance of one unit. This means $\Delta$ can be regarded as an adjacency matrix that encodes the dependencies among the electrochemical states of the ensemble. Crucially, this means electrochemical coupling depends upon the spatial relationships among the macromolecules. The corresponding rate parameters $K^{(i)} = \tfrac{1}{32}(1−exp(−4\cdot u))$; where $u \in (0,1)$ was selected from a uniform distribution to ensure topological symmetry breaking.

Similarly, the (Newtonian) motion of each macromolecule depends upon the electrochemical state of its
neighbours

$$
\begin{equation}\tag{3.2}
\begin{aligned}
  \dot{a}_n^{(i)} &= (1+\tfrac{1}{64})\mu^{(i)}s_n^{(i)}+\omega_n \\
  \dot{s}_n^{(i)} &=  2F^{(i)} - 8s_n^{(i)} - a_n^{(i)}+\omega_n \\
  \\
  F^{(i)} &= \textstyle\sum_{j=\{j:\Delta_{ij}<1\}}\Delta_{ij}\left( \cfrac{8exp(-|a_e^{(j)}-a_e^{(i)}|)-4}{\Delta_{ij}^2}-\frac{1}{\Delta_{ij}^3} \right) \\
\end{aligned}
\end{equation}
$$

This motion rests on forces $F^{(i)}$ exerted by other macromolecules that comprise a strong repulsive force (with an inverse square law) and a weaker attractive force that depends on electrochemical states. This force was chosen so that macromolecules with coherent electrochemical states are attracted to each other but repel otherwise. The remaining two terms in the second equality represent viscosity that depends upon velocity and an exogenous force that attracts all macromolecules to the origin – as if they were moving in a simple (quadratic) potential energy well. This ensures the synthetic soup falls to the bottom of the well. We now take a closer look at the self-organisation that emerges under these equations of motion.

[FIGURE 5](./img/05.png)
<p style="text-align: center;">FIGURE 5</p>

Synthetic soups and active matter. This graphic describes the equations of motion used to simulate coupled (random) dynamical systems (i.e., particles) to illustrate self-organisation. The equations describe the dynamics (that have been separated into electrochemical and Newtonian components). The schematics illustrate the conditional dependencies among particles, where each particle comprises its Markov blanket and internal states. The states with orange outlines are electrochemical states and the remaining pair constitute the Newtonian states. Note that active states (red circles) play the role of position, while sensory states (magenta circles) become velocity that depends on active states. These roles of active and sensory states will figure later, when we consider classical mechanics.

#### A random dynamical attractor and its Markov blankets

In the simulations below an ensemble of 128 particles (i.e., macromolecules) were integrated using Euler’s (forward) method with step sizes of 1/512 seconds and initial conditions sampled from a normal distribution. By adjusting the parameters in the equations of motion (3.1) and (3.2), one can produce a repertoire of plausible and interesting behaviours (the code for these simulations and the figures in this monograph are available as part of the SPM academic software – see software note). These behaviours range from gas-like behaviour (where particles occasionally get close enough to interact) to a cauldron of activity, when particles are forced together at the bottom of the potential well. In this regime, macromolecules are sufficiently close for the inverse square law to blow them apart. In other regimes, a more crystalline structure emerges with muted interactions.

However, for most values of the parameters, weakly mixing behaviour emerges, as the ensemble approaches its random global attractor (usually after about 1000 seconds). Generally, macromolecules repel each other initially and then fall back towards the centre, finding each other as they coalesce. Local interactions then mediate a self- organisation, in which particles are passed around (sometimes to the periphery) until neighbours jostle comfortably with each other. In brief, the motion and electrochemical dynamics look like an active, restless soup – but does it contain a Markov blanket?

#### The Markov blanket

Because the structural and functional dependencies share the same adjacency matrix – which depends upon position – one can use the adjacency matrix to identify the principal Markov blanket using spectral graph theory: the Markov blanket of any subset of states encoded by a binary vector with elements $\mathcal{X}_i \in \{0,1\}$ is given by $[B\cdot\mathcal{X}]\in\{0,1\}$, where the Markov blanket matrix $B=A+A^T+A^TA$ encodes the children, parents and parents of children. The principal eigenvector of the (symmetric) Markov blanket matrix will – by the Perron–Frobenius theorem – contain positive values. These values reflect the degree to which each state belongs to the cluster that is most densely coupled. In what follows, the internal particles (i.e., macromolecules) were the particles with the k = 8 largest values. Having identified internal particles, the Markov blanket can be recovered from the Markov blanket matrix using $[B\cdot\mathcal{X}]$ and divided into sensory and active particles – depending upon whether they are influenced by the external particles or not.

[FIGURE 6](./img/06.png)
<p style="text-align: center;">FIGURE 6</p>

Ensemble dynamics and self-organisation. The upper panels show the position of (128) macromolecules comprising an ensemble, after 2048 seconds. The upper left panel shows the dynamical status (three blue dots per macromolecule) of each particle centred on its location (larger dots). The ensemble of macromolecules has been partitioned into external or hidden (cyan), sensory (magenta), active (red) and internal (blue) particles. The upper right panel is an image of an endospore stain of sporulating B. Subtilis. This graphic illustrates the spatiotemporal scale at which the simulations could be operating. The lower panels show the evolution of electrochemical (middle panel) and spatial (lower panel) states of each particle as a function of time. The (electrochemical) dynamics of the internal (blue) and external (cyan) states are shown for 512 seconds. The lower panel shows the position of internal (blue) and external (cyan) states over the entire simulation period. These simulations are solutions of the stochastic differential equations in the main text – using a forward Euler method with 1/512 second time steps and random Gaussian fluctuations with a standard deviation of an eighth.

#### The emergence of order

Given the internal particles and their Markov blanket, we can now follow the assembly of constituent macromolecules and visualise their trajectories. The upper panels of Figure 6 show the position of (128) macromolecules comprising the ensemble. The upper left panel shows the electrochemical status (three blue dots per macromolecule) of each macromolecule centred on its location (larger dots) at the end of the simulation. The ensemble has been partitioned into external or hidden (cyan), sensory (magenta), active (red) and internal (blue) particles. It can be seen that the resulting Markov blanket surrounds a rod-like structure (i.e., Bacillus) of internal particles. Interestingly, the active macromolecules support the sensory macromolecules that are exposed to external particles. This is reminiscent of a biological cell with a cytoskeleton of active molecules (e.g., actin filaments), which are surrounded by sensory molecules (e.g., a cell surface). The upper right panel is an image of an endospore stain of sporulating B. Subtilis. This graphic illustrates the spatiotemporal scale at which we can imagine the simulations are operating. The lower panels show the evolution of electrochemical (middle panel) and Newtonian (lower panel) particular states as a function of time. One can see initial (chaotic) transients that resolve fairly quickly, with itinerant behaviour as they approach their attracting set. The lower panel shows the position of internal (blue) and external (cyan) particles over the entire simulation period.

Notice that something quite subtle is going on here. We started with an ensemble of particles (e.g., macromolecules), where each particle was characterised in terms of particular (i.e., sensory, active and internal) states. We then ended up with a single particle (e.g., a Bacillus or virus) characterised in terms of particular (i.e., external, sensory, active and internal) particles. In short, we have moved from a microscopic to a macroscopic scale, with blanket states at both. The next section looks more closely at this move. Here, we simply note that a macroscopic Markov blanket has emerged from simple self-organisation. So, what licenses us to describe the microscopic dynamics as self-organisation?

Figure 7 demonstrates microscopic self-organisation in terms of the particular entropy of the ensemble's particles – and concomitant changes in terms of mutual information (i.e., complexity cost or risk) and conditional entropy (i.e., ambiguity). Here, the ensemble averages of these (relative) entropy measures were taken over all (128) macromolecules; where the Markov blanket of each particle comprises all but the third (electrochemical) hidden state. This information theoretic characterisation discloses, as expected, a monotonic decrease in particular entropy (and complexity cost) as the ensemble approaches its random dynamical attractor.

#### Summary

In summary, this section has described a somewhat arbitrary random dynamical system comprising an ensemble of particles, each with several dynamical states (three electrochemical and two describing position and velocity). Crucially, the flow or equations of motion were constructed to make electrochemical coupling among the simulated macromolecules depend upon position – and render their velocity dependent upon electrochemical states. This endows the ensemble with a dynamic and sparse coupling that readily enables the emergence of a Markov blanket; separating internal from external particles (and their constituent states). In this example, the internal particles (and Markov blanket) can be thought of as modelling a little virus-like particle or rod-like bacterium. We now have at hand an in-silico creature. Later, we will examine this synthetic creature to see whether the states of internal particles (e.g., intracellular electrochemical states) plausibly infer or represent the states of external particles (e.g., extracellular motion); much as real organisms do. However, first, we need to understand how a Markov blanket emerged from the coupling of particles that were themselves constituted by Markov blankets (and their internal states).

[FIGURE 7](./img/07.png)
<p style="text-align: center;">FIGURE 7</p>

_Self-organising soups_. This demonstration uses an ensemble of particles with intrinsic (Lorentz attractor) dynamics and (Newtonian) short-range coupling to illustrate self-organisation in terms of particular (i.e., self) entropy and concomitant changes in terms of mutual information (i.e., complexity cost or risk). Here, the ensemble averages of these (relative) entropy measures were taken over all (128) particles; where the Markov blanket of each particle comprises all but the third (electrochemical) hidden state. The lower panels illustrate the decrease in blanket entropy (and complexity cost) as the system approaches its random dynamical attractor – shown as the thick and thin solid lines, respectively. The lowest broken line corresponds to conditional entropy (i.e., ambiguity). Illustrative trajectories of the particles are provided at three points during the (stochastic) chaotic transient in the upper three panels. These relative entropy changes can be compared with the equivalent results in Figure 2 for a single particle.

### States, particles and fluctuations

Let us return to where we started; namely, the Langevin equation (1.1) and ask a simple question: what is the difference between a state and a fluctuation? The answer offered in this section is that fluctuations are just fast states that change so quickly we can ignore their temporal correlations – and adopt the usual Wiener assumptions. This distinction highlights a key tenet of what is to follow; namely, a separation of temporal scales that licenses an adiabatic assumption, allowing one to separate slowly changing states from fast fluctuations. Now, let us ask a more fundamental question: what is a state? This question can be dissolved by appealing to an infinite regress along the following lines:

> What is a state? A state is an eigenstate of a particle’s Markov blanket.

> What is a particle? A particle is a set of particular states comprising blanket and internal states.

> What is a state? A state is … and so on.

An eigenstate here refers to the expression of an eigenmode of blanket states; namely, the principal eigenvectors of their Jacobian (i.e., rate of change of flow with respect to state). These mixtures are formally identical to order parameters in synergetics that reflect the amplitude of slow, unstable eigenmodes (Haken, 1983). In terms of centre manifold theory, they correspond to solutions on the slow (unstable or centre) manifold (Carr, 1981; Davis,2006)

In brief, the Markov blanket of a particle constitutes a set of vector states, whose eigenstate subtends blanket or internal states at the scale above. Note that the eigenstates are always mixtures of blanket states at the lower scale, while the eigenstates can be blanket or internal states at the higher scale. This follows from the fact that the only states ‘that matter’ are those that influence other (blanket) states. In other words, the only relevant coupling is between blanket states[^note-8]. Effectively, all we are doing here is applying the slaving principle, or centre manifold theorem (Haken, 1983), recursively to Markov blankets of Markov blankets. A complementary perspective is provided by renormalisation group approaches (Cardy, 2015; Schwabl, 2002), where the following could be seen as an attempt to establish the universality of states (and fluctuations), in the sense of constituting universality classes. The final section of Part One unpacks this construction analytically (and with numerical simulations).

[^note-8]: Relevant in the sense of renormalisation group theory: Schwabl, F., 2002. Phase Transitions, Scale Invariance, Renormalization Group Theory, and Percolation, Statistical Mechanics. Springer Berlin Heidelberg, Berlin, Heidelberg, pp.327-404.

#### Starting at the end

At a given scale or level (i) of description, we can entertain the following ansatz: a random dynamical system can be characterised as coupled subsets of states, where the n-th subset $x_n^{(i)} \subset x^{(i)}$ constitutes the vector state of a particle or nonlinear oscillator:

$$
\begin{equation}\tag{4.1}
\begin{aligned}
\dot{x}_n^{(i)} &= f_n^{(i)} + \textstyle\sum_m \lambda_{nm}^{(i)}x_m^{(i)} + \omega_n^{(i)}\\
x^{(i)} &= \{x_1^{(i)},\dots,x_N^{(i)}\} \\
\\
E[\omega_n^{(i)}(\tau)\cdot\omega_n^{(i)}(\tau^{'})] &= \begin{cases}
2\Gamma_n^{(i)}\delta(\tau - \tau^{'}) & n=m \\
0 & n \neq m
\end{cases}
\end{aligned}
\end{equation}
$$

The equations of motion for the states of the n-th particle comprise some baseline flow (at the current point in phase-space) and intrinsic and extrinsic components determined by the states of the particle in question and other particles, respectively. In this form, the diagonal elements of the coupling matrix,$\lambda_{nn}^{(i)} \in \cnums$ , determines the frequency and decay of oscillatory responses to extrinsic perturbations and random fluctuations. In what follows, we will see that (4.1) leads to an isomorphic expression for states of particles at a higher (macroscopic) scale. See Figure 8 for a schematic summary of this recursive induction.

[FIGURE 8](./img/08.png)
<p style="text-align: center;">FIGURE 8</p>

_Blankets of blankets_. This schematic illustrates the recursive procedure by which successively larger (and slower) scale dynamics arise from subordinate levels. At the bottom of the figure (lower panel), we start with an ensemble of vector states (here nine). The conditional dependencies among these vector states (i.e., eigenstates) define a particular partition into particles (upper panels). Crucially, this partition equips each particle with a bipartition into blanket and internal states, where blanket states comprise active (red) and sensory states (magenta). The behaviour of each particle can now be summarised in terms of (slow) eigenmodes or mixtures of its blanket states – to produce eigenstates at the next level or scale. These constitute an ensemble of vector states and the process starts again. Formally, one can understand this in terms of coarse graining the dynamics of a system via two operators. The first uses the particular partition to group subsets of states (**G**), while the second uses the eigenmodes of the resulting blanket states to reduce dimensionality (**R**). The upper panels illustrate the bipartition for a single particle (left panel) and an ensemble of particles; i.e., the particular partition per se (right panel). The insets on top illustrate the implicit self-similarity of particular dependencies pictorially, in moving from one scale to the next. Please see the main text for a definition of the variables used in this figure.

$$
\begin{equation}
\begin{aligned}
\dot{\pi}_j^{(i)} &= 
\begin{Bmatrix}
   \dot{a}_j^{(i)} \\
   \dot{s}_j^{(i)} \\
   \dot{\mu}_j^{(i)} \\
\end{Bmatrix} =
\begin{Bmatrix}
   f_{a_j}^{(i)}(b_j^{(i)},\mu_j^{(i)}) \\
   f_{s_j}^{(i)}(b_1^{(i)},\dots,b_j^{(i)}) \\
   f_{\mu_j}^{(i)}(b_j^{(i)},\mu_j^{(i)}) \\
\end{Bmatrix} +
\begin{Bmatrix}
   \omega_{a_j}^{(i)} \\
   \omega_{s_j}^{(i)} \\
   \omega_{\mu_j}^{(i)} \\
\end{Bmatrix} \\
\\
&= 
\begin{Bmatrix}
   \dot{b}_j^{(i)} \\
   \dot{\mu}_j^{(i)} \\
\end{Bmatrix} =
\begin{Bmatrix}
   f_{b_j}^{(i)}(\mu_j^{(i)},b_1^{(i)},\dots,b_j^{(i)}) \\
   f_{\mu_j}^{(i)}(\pi_j^{(i)}) \\
\end{Bmatrix} +
\begin{Bmatrix}
   \omega_{b_j}^{(i)} \\
   \omega_{\mu_j}^{(i)} \\
\end{Bmatrix} \\
\\
\pi^{(i)} &= \{\pi_1^{(i)},\dots,\pi_j^{(i)} \} \\
&= \{x_1^{(i)},\dots,\underbrace{\underbrace{\underbrace{x_k^{(i)},\dots,x_\ell^{(i)}}_{a_j^{(i)}},\underbrace{x_m^{(i)},\dots,x_n^{(i)}}_{s_j^{(i)}}}_{b_j^{(i)}},\underbrace{x_o^{(i)},\dots,x_p^{(i)}}_{\mu_j^{(i)}}}_{\pi_j^{(i)}},\dots,x_N^{(i)} \} \\
\end{aligned}
\end{equation}
$$

Here, active states depend only on the Markov blanket in which they participate and the internal states they
surround. Similarly, the internal states depend only upon themselves and their Markov blanket. Conversely, the
flow of sensory states depends upon all other states (apart from internal states that are sequestered behind Markov
blankets). The partition implicit in the last equality emphasises the point that a (particular) Markovian partition
is a partition into particles, where each particle is itself a partition of blanket and internal states.
Consider now the Taylor expansion of the flow of the j-th Markov blanket, where the intrinsic dynamics are
absorbed into the random fluctuations. For notational simplicity, we will assume the current state constitutes the
origin of the generalised coordinates: x 0  x (0) = 0 . So that we can express everything in terms of local
deviations:

$$
\begin{equation}\tag{4.3}
\begin{aligned}
\dot{b}_j^{(i)} &= f_{b_j}^{(i)}(b_0^{(i)})+\textstyle\sum_k J_{jk} b_k^{(i)}+\dots+K_j\varepsilon_j^{(i)}+\omega_{b_j}^{(i)} \\
\varepsilon_j^{(i)} &= \mu_j^{(i)} - \pmb{\mu}_j^{(i)}(b_j^{(i)}) \\
\\
J_{jk} &\triangleq\partial_{b_k}f_{b_j}^{(i)}(b_k^{(i)}) \\
J_{jj} &\triangleq\partial_{b_j}f_{b_j}^{(i)}(b_j^{(i)},\pmb{\mu}_j^{(i)}(b_j^{(i)})) \\
K_{j} &\triangleq\partial_{\mu_j}f_{b_j}^{(i)}(\pi_k^{(i)}) \\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{4.4}
\begin{aligned}
E[\varepsilon_j^{(i)}(\tau)\cdot \varepsilon_k^{(i)}(\tau)]=
\begin{cases}
\sum_j^{(i)} & :j=k \\
0 & :j \neq k \\
\end{cases}\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{4.5}
\begin{aligned}
J_{jk} & \triangleq \partial_{b_k} f_{b_j} =
\begin{bmatrix}
0 \\
\partial_{b_k} f_{s_j} \\
\end{bmatrix} & : j \neq k \\
K_j & \triangleq \partial_{\mu_j} f_{b_j} =
\begin{bmatrix}
\partial_{\mu_j} f_{a_j} \\
0 \\
\end{bmatrix} & : \forall j \\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{4.6}
\begin{aligned}
\pmb{\mu}_j^{(i)}(b_j^{(i)}) \triangleq E_p[\mu_j^{(i)},\dots,b_J^{(i)}] = E_p[\mu_j^{(i)}|b_j^{(i)}] \\
\end{aligned}
\end{equation}
$$

[FIGURE 9](./img/09.png)
<p style="text-align: center;">FIGURE 9</p>

$$
\begin{equation}\tag{4.7}
\begin{aligned}
\begin{bmatrix}
\lambda_{11}^{(i)} & \dots & \lambda_{1J}^{(i)} \\
\vdots & \ddots & \vdots \\
\lambda_{J1}^{(i)} & \dots & \lambda_{JJ}^{(i)} \\
\end{bmatrix} &=
\begin{bmatrix}
\xi_1^{(i)} &  \zeta_1^{(i)} \\
\vdots & \vdots \\
\xi_J^{(i)} &  \zeta_J^{(i)} \\
\end{bmatrix}^{-}
\begin{bmatrix}
J_{11} & \dots & J_{1J} \\
\vdots & \ddots & \vdots \\
J_{J1} & \dots & J_{JJ} \\
\end{bmatrix}
\begin{bmatrix}
\xi_1^{(i)} &  \zeta_1^{(i)} \\
\vdots & \vdots \\
\xi_J^{(i)} &  \zeta_J^{(i)} \\
\end{bmatrix} \\
\\
\lambda &= [\xi_j^{(i)},\zeta_j^{(i)}]^{-} J_{jj} [\xi_j^{(i)},\zeta_j^{(i)}] =
\begin{bmatrix}
\lambda_{jj}^{\xi\xi} &  0 \\
0 &  \lambda_{jj}^{\zeta\zeta} \\
\end{bmatrix} \\
\lambda &= [\xi_j^{(i)},\zeta_j^{(i)}]^{-} J_{jk} [\xi_k^{(i)},\zeta_k^{(i)}] =
\begin{bmatrix}
\lambda_{jk}^{\xi\xi} &  \lambda_{jk}^{\xi\zeta} \\
\lambda_{jk}^{\zeta\xi} &  \lambda_{jk}^{\zeta\zeta} \\
\end{bmatrix} \\
\\
[\xi_j^{(i)},\zeta_j^{(i)}]^{-}[\xi_j^{(i)},\zeta_j^{(i)}]&=I,\space\space 0 \geq Re\lambda_{jj}^{\xi\xi} \gt \epsilon \geq Re\lambda_{jj}^{\zeta\zeta}
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{4.8}
\begin{aligned}
[\xi_{j}^{(i)},\zeta_{j}^{(i)}]^{-}\dot{b}_{j}^{(i)} &=
\begin{Bmatrix}
  \xi_j^{(i)-} \dot{b}_j^{(i)} \\
  \zeta_j^{(i)-} \dot{b}_j^{(i)}
\end{Bmatrix} =
\begin{Bmatrix}
   \dot{b}_{j,slow}^{(i)} \\
   \dot{b}_{j,fast}^{(i)}
\end{Bmatrix}\\
&= \begin{Bmatrix} 
  \xi_j^{(i)-}   f_{b_j}^{(i)}(b_{0}^{(j)}) + \sum_k \lambda_{jk}^{\xi\xi}     b_{k,slow}^{(i)} \\
  \zeta_j^{(i)-} f_{b_j}^{(i)}(b_{0}^{(j)}) + \sum_k \lambda_{kj}^{\zeta\zeta} b_{k,fast}^{(i)}
\end{Bmatrix} +
\begin{Bmatrix}
  \xi_j^{(i)-}  (\omega_{b_j}^{(i)}+K_j\varepsilon_{j}^{(i)})+\sum_{k\neq j}\lambda_{jk}^{\xi\zeta} b_{k,fast}^{(i)} +\dots \\
  \zeta_j^{(i)-}(\omega_{b_j}^{(i)}+K_j\varepsilon_{j}^{(i)})+\sum_{k\neq j}\lambda_{jk}^{\zeta\xi} b_{k,slow}^{(i)} +\dots
\end{Bmatrix}\\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{4.9}
\begin{aligned}
\dot{x}_{n}^{(i)} &= f_{n}^{(i)} + \textstyle\sum_m\lambda_{nm}^{(i)}x_{m}^{(i)}+\omega_{n}^{(i)} \\
\dot{x}_{n}^{(i+1)} &= f_{n}^{(i+1)} + \textstyle\sum_m\lambda_{nm}^{(i+1)}x_{m}^{(i+1)}+\omega_{n}^{(i+1)} \\
\dot{x}_{n}^{(i+2)} &= \dots \\
\\
x_{n}^{i+1}        &\triangleq \xi_{n}^{(i)-}b_{n}^{(i)}=b_{n,slow}^{(i)} \\
f_{n}^{i+1}        &\triangleq \xi_{n}^{(i)-}f_{b_n}^{(i)}(b_{0}^{(i)}) \\
\lambda_{nm}^{i+1} &\triangleq \xi_{n}^{(i)-}j_{nm}\xi_{m}^{(i)}=\lambda_{\xi_n,\xi_m}^{(i)} \\
\omega_{n}^{i+1}   &\triangleq \xi_{n}^{(i)-}(\omega_{b_n}^{(i)}+K_n\varepsilon_{n}^{(i)})+\textstyle\sum_{k\neq n}\lambda_{nm}^{\xi\zeta} b_{m,fast}^{(i)} +\dots \\
\end{aligned}
\end{equation}
$$

[FIGURE 10](./img/10.png)
<p style="text-align: center;">FIGURE 10</p>

$$
\begin{equation}\tag{4.10}
\begin{aligned}
x^{(i)} &=\{ x_1^{(i)},\dots,
  \underbrace{
    \underbrace{x_k^{(i)},\dots,x_\ell^{(i)}}_{a_{j}^{(i)}},
    \underbrace{x_m^{(i)},\dots,x_n^{(i)}}_{s_{j}^{(i)}}
  }_{b_{j}^{(i)}},
    \underbrace{x_o^{(i)},\dots,x_p^{(i)}}_{\mu_{j}^{(i)}},
    \dots,x_N^{(i)},\} \\
x_{n}^{(i+1)} &= \xi_{n}^{(i)-} b_{n}^{(i)}
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{4.11}
\begin{aligned}
\omega_{n}^{(i+1)} &= \xi_{n}^{(i)-}(K_{n}^{(i)}\varepsilon_{n}^{(i)} + \omega_{b_n}^{(i)}) \\
\omega_{b_{n_j}}^{(i)} &= \xi_{b_{n_j}}^{(i-1)-}(K_{b_{n_j}}^{(i-1)}\varepsilon_{b_{n_j}}^{(i-1)}+\omega_{b_{n_j}}^{(i-1)}) \\
&\space\space\vdots
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{4.12}
\begin{aligned}
\mathcal{L}(x_{n}^{(i)},\dot{x}_{n}^{(i)}) & = \tfrac{1}{2}[(\dot{x}_{n}^{(i)}-\phi_{n}^{(i)})\cdot(2\Gamma_{n}^{(i)})^{-1}(\dot{x}_{n}^{(i)}-\phi_{n}^{(i)})+\nabla\cdot\phi_{n}^{(i)}] \\
\phi_{n}^{(i)} &= f_{n}^{(i)}+\textstyle\sum_m\lambda_{nm}^{(i)} x_{m}^{(i)} \\
\\
\{x_{n}^{(i)}\} &= \pmb{R}\circ\pmb{G}\circ\{x_{n}^{(i-1)}\} \\
\{f_{n}^{(i)},\lambda_{nm}^{(i)},\Gamma_{n}^{(i)}\} &= \beta(\{f_{n}^{(i-1)},\lambda_{nm}^{(i-1)},\Gamma_{n}^{(i-1)}\})
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{4.13}
\begin{aligned}
\xi_{n}^{(i)}         &\rightarrow \xi_{n}^{(i)} \Rightarrow \xi_{n}^{(i)-}(K_{n}^{(i)}\Sigma_{n}^{(i)} K_{n}^{(i)T} + 2\Gamma_{b_n}^{(i)})\xi_{n}^{(i)} = 2\Gamma_{n}^{(i+1)} \\
\{x_{n}^{(i)}\}       &\xrightarrow{G}      \{b_{j}^{(i)}\} \subset\{b_{j}^{(i)},\mu_{j}^{(i)}\} \\
\\
\{b_{n}^{(i)}\}       &\xrightarrow{R}      \{x_{n}^{(i+1)}\} = \{\xi_{n}^{(i)-} b_{n}^{(i)}\} \\
\{f_{n}^{(i)}\}       &\xrightarrow{\beta}  \{f_{n}^{(i+1)}\} = \{\xi_{n}^{(i)} - f\} \\
\{\lambda_{nm}^{(i)}\}&\xrightarrow{\beta}  \{\lambda_{nm}^{(i+1)}\} = \{\xi_{n}^{(i)-}\partial_{b_m} f_{b_n}^{(i)} \xi_{m}^{(i)} \} \\
\{\Gamma_{n}^{(i)}\}  &\xrightarrow{\beta}  \{\Gamma_{n}^{(i+1)}\} = \{\xi_{n}^{(i)-}(\Gamma_{n}^{(i)}+\tfrac{1}{2}\partial_{\mu_n} f_{b_n}^{(i)} \Sigma_{b_n}^{(i)} \partial_{\mu_n} f_{b_n}^{(i)T})\xi_{n}^{(i)} \} \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{4.14}
\begin{aligned}
E[Re(\lambda_{nn}^{(i)})] \leq E[Re(\lambda_{nn}^{(i+1)})]\dots\leq 0 \\
\end{aligned}
\end{equation}
$$

[FIGURE 11](./img/11.png)
<p style="text-align: center;">FIGURE 11</p>

[FIGURE 12](./img/12.png)
<p style="text-align: center;">FIGURE 12</p>

$$
\begin{equation}\tag{5.1}
\begin{aligned}
p    &= \Psi \cdot \Psi \\
\Psi &= \Psi(x)e^{-iEt/\hbar}
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.2}
\begin{aligned}
\pmb{H}\Psi &= E\Psi \\
\pmb{H}     &= V(x)-\tfrac{\hbar^2}{2m}\cdot\nabla^2 \\
V(x)        &= \tfrac{m}{2}f\cdot f + \tfrac{\hbar}{2}\nabla\cdot f \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.3}
\begin{aligned}
\Gamma     &= \tfrac{\hbar}{2m} \\
p          &= \Psi^{\dagger}\Psi \\
f          &= \tfrac{\hbar}{2m}\nabla\ln{p}=-\Gamma\nabla\Im \Rightarrow \\
pf         &= \tfrac{\hbar}{2m}\nabla p = \tfrac{\hbar}{2m}\nabla(\Psi\cdot\Psi^{\dagger}) \Rightarrow \\
\Psi^{\dagger}f\Psi &= \tfrac{\hbar}{2m}(\Psi^{\dagger}\nabla\Psi+\Psi\nabla\Psi^{\dagger}) \Rightarrow \\
\nabla\Psi &= \tfrac{m}{\hbar}f\Psi \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.4}
\begin{aligned}
\dot{p} &= \tfrac{\hbar}{2m}\nabla^2 p - p\nabla\cdot f - f \cdot \nabla p \\
        &= \tfrac{\hbar}{2m}\nabla^2\Psi^{\dagger}\Psi 
           - \tfrac{1}{2}\Psi\nabla\cdot f\Psi^{\dagger} 
           - \tfrac{1}{2}\Psi^{\dagger}\nabla\cdot f\Psi
           - \Psi f\cdot\nabla\Psi^{\dagger} 
           - \Psi^{\dagger} f \cdot\nabla\Psi \\
        &= (\tfrac{\hbar}{2m}\nabla^2)+(\tfrac{\hbar}{2m}\nabla^2) \\
        \\
V(x)    &= \tfrac{m}{2}f\cdot f+\tfrac{\hbar}{2}\cdot f \\
        &= \tfrac{\hbar^{2}}{4m}(\tfrac{1}{2}\nabla\Im\cdot\nabla\Im-\nabla^2\Im)
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.5}
\begin{aligned}
i\hbar\dot{p} &= \Psi^{\dagger}i\hbar\Psi + \Psi i\hbar\Psi = \Psi^{\dagger}E\Psi - \Psi E\Psi^{\dagger} = 0 \\
-\hbar\dot{p} &= \Psi^{\dagger}\pmb{H}\Psi + \Psi\pmb{H}\Psi^{\dagger} = 0 \\
\pmb{H}       &= V(x) - \tfrac{\hbar^2}{2m}\nabla^2 \\
              &\Leftarrow \\
\pmb{H}\Psi   &= i\hbar\dot{\Psi} = E\Psi \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.6}
\begin{aligned}
\dot{p} &= \pmb{L}p(x) \\
\pmb{L} &= \tfrac{\hbar}{2m}\nabla^2 - \nabla\cdot f \\
\\
i\hbar\dot{\Psi}(x) &= \pmb{H}\Psi(x) \\
-\tfrac{1}{\hbar}\pmb{H} &= \tfrac{\hbar}{2m}\nabla^2 - \tfrac{1}{\hbar}V(x) \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.7}
\begin{aligned}
\Psi(x,t) &= \Psi(x)e^{-i\omega t} = \Psi(x)^{-iEt/\hbar} \\
\Psi(x)   &= \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}\Phi(k)\cdot e^{ik\cdot x}dk \\
\Phi(k)   &= \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}\Psi(x)\cdot e^{-ik\cdot x}dk \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.8}
\begin{aligned}
\braket{\Psi^{\dagger}(x)|-i\hbar\nabla|\Psi(x)} 
  &= -i\hbar\int_{-\infty}^{\infty} \Psi(x)^{\dagger}\nabla\Psi(x)dx \\
  &= -i\hbar\int_{-\infty}^{\infty} \Psi^{\dagger}\frac{m}{\hbar}f\Psi(x)dx = -imf\\
  &= \braket{\Phi(k)^{\dagger}|\hbar k|\Phi(k)} = \hbar k \Rightarrow mf = i\hbar k \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.9}
\begin{aligned}
\pmb{H}\Psi &= i\hbar\Psi = h\omega\Psi = E\Psi \\
\pmb{p}\Psi &= -i\hbar\nabla\Psi = \hbar k\Psi \\
\\
E &\triangleq \hbar\omega \\
p &\triangleq \hbar \pmb{k} = m\pmb{f} \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.10}
\begin{aligned}
\pmb{H} &= \pmb{T}+V(x) \\
\pmb{T} &= \tfrac{1}{2m}\pmb{p}\cdot \pmb{p} = -\tfrac{\hbar^2}{2m}\cdot\nabla^2 \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.11}
\begin{aligned}
\braket{\Psi^{\dagger}|\pmb{H}|\Psi}
  &= \underbrace{\braket{\Psi^{\dagger}|\pmb{T}|\Psi}}_{\text{kinetic energy}}
  +  \underbrace{\braket{\Psi^{\dagger}|V(x)|\Psi}}_{\text{potential energy}} \\
  &= \underbrace{\tfrac{m}{2}\braket{f\cdot f}}_{\text{kinetic energy}}
  +  \underbrace{\braket{\tfrac{m}{2} f\cdot f + \tfrac{\hbar}{2}\nabla\cdot f}}_{\text{potential energy}} = E \\
\\
\braket{\nabla\cdot f}
  &= -\Gamma\braket{\nabla^2\Im} = -\Gamma\braket{\nabla\Im\cdot\nabla\Im} = -\tfrac{2m}{\hbar}\braket{f\cdot f}
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.12}
\begin{aligned}
f(x)=c \Rightarrow E = mc^2 \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.13}
\begin{aligned}
\sigma_x\sigma_p \geq \tfrac{\hbar}{2} \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.14}
\begin{aligned}
\Sigma_x\Sigma_p 
  &= E[x\cdot x]E[mf\cdot mf] \\
  &= (\tfrac{\hbar}{2})^2 \Sigma_x^{-2}E[x\cdot x]E[x\cdot x] = (\tfrac{\hbar}{2})^2 \\
  \\
\Im(x)
  &= \tfrac{1}{2}x\cdot \Sigma_x^{-1}\cdot x \\
f(x)
  &= -\tfrac{\hbar}{2m}\nabla\Im = \tfrac{\hbar}{2m}\nabla^2\Im\cdot x \\
\Sigma_x^{-1}
  &= -\nabla^2\Im \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{5.15}
\begin{aligned}
\Gamma
  &= \tfrac{\hbar}{2m},\space\space\space V(x) = -\tfrac{\hbar^2}{a_0 m_e r} \\
  \\
\Psi_{n\ell m}(x)
  &= \sqrt{Z}e^{\rho/2} \rho^\ell L_{n-\ell-1}^{\ell+\ell+1}(\rho)Y_\ell^m (\theta,\phi) \\
\rho
  &= \tfrac{2r}{na_0},\space\space\space Z = (\tfrac{2}{na_0})^3\tfrac{n-\ell-1}{2n(n+\ell)!}
\end{aligned}
\end{equation}
$$

[FIGURE 13](./img/13.png)
<p style="text-align: center;">FIGURE 13</p>

[TABLE 2](./img/t2.png)

$$
\begin{equation}\tag{6.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{6.20}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{7.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{7.15}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{8.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{8.33}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{9.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{10.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{10.12}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{11.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{11.3}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{12.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{12.16}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{13.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{13.3}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{14.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{14.10}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{15.1}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$
$$
\begin{equation}\tag{15.5}
\begin{aligned}
\\
\end{aligned}
\end{equation}
$$

#### The adiabatic reduction
#### Elimination and renormalisation
#### Summary

## Part 2: some special cases
## Part 3: a particular case

## Discussion
### Conclusions

## Appendix A: Stratonovich path integrals
## Appendix B: lemmas and proofs
## Appendix C: nonequilibrium steady-static energy functions
## Appendix D: the Fokker-Planck operator
## Appendix E: generalised motion
## Appendix F: discrete state-space models

## References
