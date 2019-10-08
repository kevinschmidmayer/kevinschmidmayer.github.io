---

layout: page
title: Start
permalink: /start/
---

<article>
	<h2> Installation guide </h2>
	<div> 
		<h3> Prerequisites </h3>
		<p> ECOGEN must be compiled with <b>C++</b>. It also requires a functional system implementation of <b>MPI library</b> (not provided in this package). Depending on your operating system, click on the corresponding link below to obtain additional information: 
		</p>
		<p> Installation prerequisites for <a href="{{ "/prerequisitesUbuntu" | prepend: site.baseurl }}"> Ubuntu system / Windows 10 using bash</a> (<em>Ubuntu on Windows App</em>). </p>
		<p> Installation prerequisites for <a href="{{ "/instalOnWindows" | prepend: site.baseurl }}"> Windows system </a>. </p>
	</div>	
	<div> 
		<h3> Download ECOGEN </h3>
		<p> The last ECOGEN version can be downloaded from GitHub. The source files are available at the following address: 
        <a href="https://github.com/code-mphi/ECOGEN" target="_blank" >https://github.com/code-mphi/ECOGEN</a>.
        </p>
	</div>
	<div> 
		<h3> Compilation/Execution on bash (Ubuntu or Windows) </h3>
		<p> Use the Makefile (can be adapted if necessary) to compile ECOGEN sources directly on bash (XX is the number of cores required for compilation): </p> 
		<div class="cmd">make -j XX </div>
		<p> Executing ECOGEN is really easy on bash (XX is the number of cores required for execution): </p>
		<div class="cmd">mpirun -np XX ECOGEN </div> 
	</div>
</article>

<article>
	<h2> First use of ECOGEN </h2>
	<p> 
		Tutorials are available on the <a href="https://code-mphi.github.io/ECOGEN/docs/sphinx_docs/Chap4_1startWithECOGEN.html" target="_blank" >official documentation</a> website.
	</p>
</article>
