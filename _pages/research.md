---
layout: page
title: Research
permalink: /research/
---

<article>
	<p> My work is generally devoted to the modelling, the development of numerical methods, the simulation and the analysis of multiphysics, multiphase, compressible flows. In the following are presented some of my research works:
	<ul>
		<li> <a href="#anchor-ECOGEN"> ECOGEN: open-source tool dedicated to multiphase compressible multiphysics flows. </a> </li>
		<li> <a href="#anchor-shock-induced-cavitation"> Shock-induced cavitation within a droplet. </a> </li>
		<li> <a href="#anchor-bubble-dynamics"> Bubble dynamics and cavitation in medicine. </a> </li>
		<li> <a href="#anchor-aerobreakup"> Water-droplet and water-column aerobreakup. </a> </li>
		<li> <a href="#anchor-heat-exchanger"> Heat exchanger with dynamic wall. </a> </li>
		<li> <a href="#anchor-density-currents"> Sediment-laden density currents propagating down slopes into stratified ambient. </a> </li>
	</ul>
	</p>
</article>

<article>
	<h1 id="anchor-ECOGEN"> ECOGEN: open-source tool dedicated to multiphase compressible multiphysics flows </h1>
	<p> ECOGEN is C++ code under an open-source GNU license developped by multiphase-compressible-flow researchers and has vocation to treat:
		<ol>
			<li> Cartesian or unstructured meshes with or without AMR, </li>
			<li> High-order numerical method based on Finite Volume method, </li>
			<li> Single or multiphase compressible flows, </li>
			<li> Multiphysics such as:
				<ul>
					<li> Surface tension, </li>
					<li> Viscosity, </li>
					<li> Heat conduction, </li>
					<li> Phase transition, </li>
					<li> Cavitation, </li>
					<li> Solids mechanics. </li>
				</ul>
			</li>
		</ol>
	</p>
	<p style="text-align:center;">Access ECOGEN's website:</p>
	<div class="buttonECOGEN"> 
		<a href="https://code-mphi.github.io/ECOGEN/" target="_blank"> <img src="{{ "/assets/images/transparent.png" | prepend: site.baseurl }}" alt="get it now!" /> </a> 
	</div>
</article>

<article>
	<h1 id="anchor-shock-induced-cavitation"> Shock-induced cavitation within a droplet </h1>
	<p> Investigations of shock-induced cavitation within a droplet are highly challenged by the multiphase nature of the mechanisms involved. Within the context of heterogeneous nucleation, we introduced a thermodynamically well-posed multiphase numerical model accounting for phase compression and expansion, which relies on a finite pressure-relaxation rate formulation. We simulated (i) the interaction of a cylindrical water droplet with a planar shock wave, and (ii) the high-speed impact of a gelatin droplet onto a solid surface. The determination of the finite pressure-relaxation rate was done by comparing the numerical results with the corresponding experiments of Sembian et al. and Field et al., respectively. Upon the validation of the determined pressure-relaxation rate, we ran parametric simulations to elucidate the critical Mach number from which cavitation is likely to occur. Complementing simulations with a geometrical acoustic model, we provided a phenomenological description of the shock-induced cavitation within a droplet, as well as a discussion on the bubble-cloud growth effect on the droplet flow field. The usual prediction of the bubble cloud center, given in the literature, was eventually modified to account for the expansion wave magnitude.
	</p>
	<center><img src="{{ "/assets/images/shock-induced_cavitation_phenomenology.png" | prepend: site.baseurl }}" alt="shock-induced_cavitation_phenomenology" style="width: 100%; height: 100%;" /></center>
	<figcaption>Sketch of the internal wave pattern and phenomenology of the shock-induced cavitation within a liquid droplet. Time is indicated with a red-to-blue colormap, with t=0 the instant at which the incident shock reaches the droplet. Not all internal reflections are drawn for the sake of clarity and educational purposes.</figcaption>
	<p> </p>
	<center><img src="{{ "/assets/images/shock-induced_cavitation_comparison.png" | prepend: site.baseurl }}" alt="shock-induced_cavitation_comparison" style="width: 100%; height: 100%;" /></center>
	<figcaption>Comparison of the internal droplet structure between (top) numerical simulations at different μ and (bottom) the experiment of Sembian et al. The upper-halves display the volume fraction of air (yellow-to-black colormap) overlaid with numerical Schlieren images (white). The lower-halves disclose experimental Schlieren images. The dashed red line on the fifth frame contours the bubble cloud as indicated in Sembian et al.</figcaption>
</article>

<article>
	<h1 id="anchor-bubble-dynamics"> Bubble dynamics and cavitation in medicine </h1>
	<p> Work on models and numerical methods, in the diffuse-interface framework, able to treat as best bubble dynamics and cavitation has been done. Following this work and through numerous and close collaborations with experimentalists, numericians and theoreticians from different international universities and companies, interesting biomedical problems can be investigated such as: The impact of a collapsing gas bubble above rigid, flat or notched walls mimicking the surface of urinary stones during lithotripsy or more generally to assess cavitation-induced erosion. The collapse of cavitation bubbles located within the syringe cone of autoinjector devices and resulting in stresses large enough to cause syringe failure. The characterization of viscoelastic materials (biomaterials) at high strain rates, induced by the cavitation bubbles, via ensemble-based data assimilation of bubble collapse observations.
	</p>
	<center><img src="{{ "/assets/images/bubbleDyn_kidneyStone.png" | prepend: site.baseurl }}" alt="bubbleDyn_kidneyStone" style="width: 85%; height: 85%;" /></center>
	<figcaption>Collapse of a microbubble at the surface of urinary stone. On the left, image of a kidney stone. On the right, snapshots of experimental (a) and simulation (b) results. In (b), the upper half shows pressure in color on a logarithmic scale and the color image is overlaid by the volume fraction of gas shown in black and white, with an opacity function to render translucent surfaces. The black shows regions of high gas content. The opaqueness decreases with volume fraction until the gas volume fraction is zero (100% liquid) depicted as 100% transparent. The lower half shows numerical schlieren.</figcaption>
	<p> </p>
	<center><img class= "galleryGif" src="{{ "/assets/images/bubble_collapse_crevice.gif" | prepend: site.baseurl }}" alt="bubble_collapse_crevice" style="width: 70%; height: 70%;" /></center>
	<figcaption>Numerical schlieren (left) and log-scale pressure fields (right) of an air bubble collapsing onto a wall with a small crevice RC/R0 = 0.15 and of stand-off distances S/R0 = 0.6. Gas volume fraction is shown as a shaded area of decreasing opacity with decreasing volume fraction (left), while the isoline of volume fraction equal to 0.5 is shown as a solid curve (right) representing a pseudo-phase interface.</figcaption>
</article>

<article>
	<h1 id="anchor-aerobreakup"> Water-droplet and water-column aerobreakup </h1>
	<p> A new model and numerical method have been proposed to solve multiphase compressible flows with surface tension:
		This new model is in agreement with physical principles of conservation, respects the second law of thermodynamics and is shown hyperbolic in a 3D framework. A new numerical method is also proposed where the global system of equations is split into several submodels. Each submodel is hyperbolic and can be solved with an adequate numerical method. The surface-tension effects were earlier validated thanks to comparison with analytical solutions (Laplace law) and has been shown to give better results than the traditional source-term-integration method. The simulations are also using a new Adaptive Mesh Refinement method (AMR) method. The water-droplet and water-column breakup is made by a high-speed flow behind a shock wave to therefore proceed to the atomization.
	</p>
	<center><img src="{{ "/assets/images/3Datom_mesh.png" | prepend: site.baseurl }}" alt="3Datom_mesh" style="width: 75%; height: 75%;" /></center>
	<figcaption>Snapshot of water-droplet atomization. Visualization of vorticity contour on the upper half with velocity-magnitude colors (high velocity in red and low velocity in blue) and visualization of the AMR mesh on the lower half colored by the different cores used (adaptive parallel load balancing is used).</figcaption>
	<p> </p>
	<center><iframe src="https://player.vimeo.com/video/365286902" width="640" height="331" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></center>
	<figcaption>Water-droplet atomization. Visualization of volume-fraction contour on the left and vorticity contour on the right with velocity-magnitude colors (high velocity in red and low velocity in blue).</figcaption>
	<p> </p>
	<center><iframe src="https://player.vimeo.com/video/169677099" width="512" height="288" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></center>
	<figcaption>Early stages of a water-column breakup by a shock wave. Wave propagation is shown through a schlieren visualization (function of the mixture-density gradient).</figcaption>
	<p> </p>
	<center><iframe src="https://player.vimeo.com/video/365306429" width="640" height="400" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></center>
	<figcaption>Atomization of a water column by a high-speed flow propagating from the left to the right and induced by a shock wave. On the upper half, the water is shown in red and the mist of micrometer water droplets is shown in blue. On the lower half, vorticity is shown.</figcaption>
</article>

<article>
	<h1 id="anchor-heat-exchanger"> Heat exchanger with dynamic wall </h1>
	<p> Compactness, efficiency and control of heat exchangers are of great interest in many processes. A technological breakthrough must be achieved to go further in their ability to respond to the needs. In this view, a new concept of heat exchanger at millimeter scale has been proposed. It consists in dynamically deforming at least one of the walls in order to obtain a progressive corrugated channel.
	</p>
	<p> Systematic studies were performed in single-phase flow on the different deformation parameters that allow obtaining the flow and heat-transfer characteristics of the system. The optimum operating conditions for thermal control of electronic components are determined. It has been observed the dynamic wall deformation induces a significant pumping effect. Intensification of heat transfer remains very important even for highly degraded waveforms although the pumping efficiency is reduced in this case.
	</p>
	<center><img src="{{ "/assets/images/heatExchanger_mesh.jpg" | prepend: site.baseurl }}" alt="heatExchanger_mesh" style="width: 65%; height: 65%;" /></center>
	<center><img src="{{ "/assets/images/heatExchanger_temperature.jpg" | prepend: site.baseurl }}" alt="heatExchanger_temperature" style="width: 95%; height: 95%;" /></center>
</article>

<article>
	<h1 id="anchor-density-currents"> Sediment-laden density currents propagating down slopes into stratified ambient </h1>
	<center><img src="{{ "/assets/images/turbidity_3D.png" | prepend: site.baseurl }}" alt="turbidity_3D" style="width: 90%; height: 90%;" /></center>
	<p> Intrusions can form when sediment-laden gravity currents propagate down the continental slope into the density stratified ambient ocean. As the particles settle from the initially bottom propagating sediment-laden current, its bulk density decreases, and it eventually lifts off the ground to propagate as an intrusion current. Numerical simulations have been performed to study such currents in the lock-exchange configuration. The flow characteristics of the currents, such as their front speed, their lift-off location and their deposit profiles were analyzed as functions of particle size, ambient strength and Reynolds number. As a general trend, currents with larger particles lift off earlier to form intrusions, and they propagate closer to the top surface as compared to currents with smaller particles. Comparison of our simulation results with laboratory experiments of Snow and Sutherland (2014) were shown.
	</p>
	<center><img src="{{ "/assets/images/turbidity_comparisonExp.png" | prepend: site.baseurl }}" alt="turbidity_comparisonExp" /></center>
</article>
