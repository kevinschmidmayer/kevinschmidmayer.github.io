---

layout: page
title: Gallery
permalink: /gallery/
videoErrormessage: Sorry, your browser does not support webm video format or video HTML element.
---
<div>
	<p>
		There are multiple ways to use ECOGEN for simulating single or multiphase flows. Hereafter are presented some recent applications involving different physical effects.
	</p>
	<article>
		<h2> Physics of Shock </h2>
		<p> Shock waves can propagate in matter whatever its physical state:  Gaseous, liquid or even solid. They can travel through interfaces or into a multiphase mixture of materials. Because ECOGEN is devoted to compressible, hyperbolic systems of equations, shock dynamics is included whatever the problem is. </p>
		<div class="gallery">
			<div class="galleryVideo">
				Shock-wave propagation in ducts is a challenging problem for safety issues. Such studies are performed to improve the safety in confined installation thanks to a better knowledge of the pressure-wave characteristics. In this movie, the shock-wave propagation in a "Y" bifurcation channel is shown: Because of the bifurcation, the amplitude of the incident pressure jump is expected to decrease in the secondary ducts.
			</div>
			<div class="galleryVideo">
				<video  src="{{ "/assets/videos/chocs.webm" | prepend: site.baseurl }}" controls preload >{{ page.videoErrormessage}}	</video>
				<figcaption>Shock-wave propagation in a channel junction (A. Marty courtesy).</figcaption>
			</div>
		</div>		
		<div class="gallery">
			<div class="galleryVideo">
				<video  src="{{ "/assets/videos/shockHeliumBubble_forFun_highResolution_2.webm" | prepend: site.baseurl }}" controls preload >{{ page.videoErrormessage}}</video>
				<figcaption>Interaction shock wave / helium bubble<br>
				Upper half: Volume fraction <br>
				Lower half: Numerical schlieren (shows interfaces and shocks) </figcaption>
			</div>
			<div class="galleryVideo">
				This video illustrates the shock/bubble interaction: The bubble contains lighter fluid (He) than the surrounding gas (air). Richtmyer-Meshkov instabilities deform the interface where the pressure and density gradients generate vorticity. Main parameters of the flow pattern are the acoustic impedance and so indirectly the speed of sound of both fluids.
			</div>
		</div>
	</article>
	<hr> 
	<article>
		<h2> Cavitation </h2>
		<p> The ability to treat cavitation problems is definitely one of the major assets of the diffuse-interface formulation. Now, thanks to consistent thermodynamics consideration, it is possible to intrinsically simulate interface appearance / disappearance between a liquid and its vapor without any specific algorithm for interface tracking. </p>
		<div class="gallery">
			<div class="galleryVideo">
				<video  src="{{ "/assets/videos/bubbleCollapse.webm" | prepend: site.baseurl }}" controls preload>{{ page.videoErrormessage}}</video>
				<figcaption>Bubble collapse near a wall. Courtesy of Caltech, MCE. </figcaption>
			</div>
			<div class="galleryVideo">
				Collapse of an ellipsoidal microbubble attached to a flat rigid surface for studying minimally invasive treatment of urinary stones. The simulation is 2D axisymmetric. Left panel shows pressure in color overlaid by the volume fraction of gas (upper half) and numerical schlieren of mixture-density gradients (lower half). Right panel shows maximum pressure at the rigid wall.
			</div>
		</div>		
		<div class="gallery">
			<div class="galleryVideo">
				This very complex flow shows two major phenomena due to a high-speed bubble of water impacting a wall (on the left): A right-moving shock wave is created. One can then observe the typical interaction of a bubble that contains heavy fluid (water) in a lighter fluid (air) with Richtmyer-Meshkov instabilities. The impact on the wall also creates left-moving expansion waves leading to the appearance of cavitation pockets due to the decreasing pressure.
			</div>				
			<div class="galleryVideo">
				<video src="{{ "/assets/videos/rycht.webm" | prepend: site.baseurl }}" controls preload>{{ page.videoErrormessage}}</video>
				<figcaption>Water/air Richtmyer-Meshkov instability</figcaption>
			</div>
		</div>
	</article>
	<hr> 
	<article>
		<h2> Droplet fragmentation </h2>
		<p> The simulation of droplet fragmentation is of prime interest considering various industrial applications as well as for academic knowledge. The deformation of the droplet is a competition between surface tension and inertial forces (measured by the Weber number) that can lead to the creation of smaller droplets. Surface tension then determines the resulting droplet sizes. </p>
		<div class="gallery">
			<div class="galleryVideo">
				<video src="{{ "/assets/videos/atomization3D.webm" | prepend: site.baseurl }}" controls preload>{{ page.videoErrormessage}}</video>
				<figcaption>Fragmentation of a droplet in a high-speed flow</figcaption>
			</div>
			<div class="galleryVideo">
				The movie shows a water-droplet atomization by the high-speed flow produced by a shock wave at Mach 1.3. Contours, using water volume fraction equal to 10e-3 and mixture-velocity-norm colormap (dark red shows strong mixture-velocity norms and dark blue shows small ones), are shown to observe filaments and potential reduced-size droplets.
			</div>	
		</div>
		<div class="gallery">
			<div class="galleryVideo">
				In this movie, a liquid droplet is moving in a box with perfect solid walls. At the impact on the upper wall, the bubble is sliding, deforming then dividing in smaller droplets. Due to the gravity, some small droplets fall down while a droplet is sliding down along the vertical wall. One can observe the rebounds of the droplets as well as the various droplet/droplet interactions leading to coalescence phenomena.
			</div>	
			<div class="galleryVideo">
				<video src="{{ "/assets/videos/movie_V1.webm" | prepend: site.baseurl }}" controls preload>{{ page.videoErrormessage}}</video>
				<figcaption>Motion and fragmentation of a liquid droplet in a box with solid walls. <br>
				Simulation including surface-tension effects and gravity. </figcaption>
			</div>
		</div>
	</article>

</div>
