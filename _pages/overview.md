---

layout: page
title: Overview
permalink: /overview/
---
<div class="colonne">
	<aside>
		<h2> Sharing knowledge </h2>
			<p>ECOGEN is a CFD platform dedicated to numerical simulation of compressible multiphase flows. It has the vocation to share academics researches in the multiphase flow field with other academics but also with industrials, students, etc.
			<ul>  
				<li> Multi-models (single phase, multiphase with or without equilibrium). </li>
				<li> Multi-physics (thermal transfers, viscosity, surface tension, mass transfers). </li>
				<li> Multi-meshes (Cartesian, unstructured, AMR). </li>
				<li> Multi-cores. </li>
			</ul>
			</p>
		<h2> Features </h2>
		<ul>		
			<li> Solves interface problems between pure or multicomponent fluids and mixtures of multiphase flows. </li>
			<li> Treats surface tension, heat and mass transfers for cavitation and evaporating and condensing flows. </li>
			<li> Computes wave propagation in strongly unsteady situations using a specific Adaptive Mesh Refinement. </li>
			<li> C++ object oriented programming language. </li>
			<li> Computes unstructured grids to simulate complex geometries. </li>
			<li> Parallel computing using open MPI libraries. </li>			
		</ul>	
	</aside>
	<div>
		<article>
			<h2> <span class="lettre">E</span>COGEN is Evolutive </h2>
			<p>Academic research results never represent achievements but rather step forwards. This is all the more noticeable in the young discipline of numerical sciences where models and methods are in constant evolution to better represent physical phenomena. In the structure of ECOGEN, the modular aspect of C++ programming language has been used to help developing future evolutions. </p>
			<img src="{{ "/assets/images/mainClasses.png" | prepend: site.baseurl }}" alt="general ECOGEN structure" />
			<p>Thanks to that, it becomes easy for developers to add a new equation of state or a flow model. </p>
		</article>
		<article>
			<h2> E<span class="lettre">C</span>OGEN is designed for Compressible flows </h2>
			<p>Compressible information is transmitted thanks to wave propagation. Mathematical systems of equations modeling compressible flows present hyperbolic formulations that should be specifically treated numerically. </p>
			<div class="flex">
				<img src="{{ "/assets/images/shocks.png" | prepend: site.baseurl }}" alt="shock waves" />
				<p>ECOGEN is designed for such compressible flows. </p>
			</div>
		</article>
		<article>
			<h2> EC<span class="lettre">O</span>GEN is Open Source </h2>
			<p>ECOGEN is an open-source project distributed under <a href="https://www.gnu.org/licenses/gpl-3.0.en.html" target="_blank" > GNU GPLv3 License </a> and available on <a href="https://github.com/code-mphi/ECOGEN" target="_blank" > GitHub</a>. Interested developers are encouraged to contribute in the project. </p>
		</article>
		<article>
			<h2> ECO<span class="lettre">G</span>EN is Genuine </h2>
			<div class="flex">
				<p>Existing CFD codes can treat multiphase flows, but ECOGEN is the first to use the diffuse-interface theory to dynamically capture the complex shapes of multiphase flows on structured or unstructured grids. Moreover, it includes an Adaptive Mesh Refinement (AMR) method for Cartesian grids specifically developed and optimized for such multiphase flows. </p>
				<img src="{{ "/assets/images/maillage.png" | prepend: site.baseurl }}" alt="mesh" />
			</div>
		</article>
		<article>
			<h2> ECOG<span class="lettre">E</span>N is Easy </h2>
			<p>All you need is a C++ compiler running with Message Passing Interface (MPI) library to use ECOGEN. The standard VTK file format used for results makes the post-treatment flexible. Just follow the tutorials and compute! </p>
		</article>	
		<article>
			<h2> ECOGE<span class="lettre">N</span> is N-phase </h2>
			<p>Even if ECOGEN is able to solve single-phase gas or compressible liquid dynamics, it reveals its power when a flow is composed with an arbitrary number of phases. If you can now simulate a liquid phase with its vapor, there is no difficulty to add one or several inert phases in the flow. </p>
		</article>
	</div>
</div>