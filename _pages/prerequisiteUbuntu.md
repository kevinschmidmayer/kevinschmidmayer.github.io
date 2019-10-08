---
layout: page
title: Prerequisites Ubuntu
permalink: /prerequisitesUbuntu/
---

<p> ECOGEN required two mandatory components to be installed on your Ubuntu system: A C++ compiler and an effective implementation of MPI. You can follow the proposed tutorials to set a complete open-source installation hereafter. </p>

<article>
	<h2> Installing a C++ compiler </h2>
	<div> 
		<p> Nothing is easier than installing C and C++ compiler on Ubuntu. </p>
		<div class="cmd"> sudo apt-get update<br>
			sudo apt-get upgrade<br>
			sudo apt-get install gcc<br>
			sudo apt-get install g++<br>
			sudo apt-get install build-essential<br>
		</div>
		<p> More information on the Ubuntu documentation page <a href="https://doc.ubuntu-fr.org/gcc" target="_blank">https://doc.ubuntu-fr.org/gcc</a> </p>
	</div>	


</article>

<article>
	<h2> Installing openMPI </h2>
	<div> 
		<p> Download the latest stable version of <a href="https://www.open-mpi.org/" target="_blank">openMPI</a> under compressed format. At the time this page is written, it corresponds to the compressed file: openmpi-4.0.1.tar.gz. Uncompress and move into the directory: </p>
		<div class="cmd">
			tar -xvf openmpi-4.0.1.tar.gz <br>
			cd openmpi-4.0.1/
		</div>
		<p> Prepare the environment to use your favorite compiler: </p>
		<div class="cmd">
			export CC=gcc <br>
			export CXX=g++ <br>
		</div>
		<p> Configure and proceed to the installation (you can choose a different directory): </p>
		<div class="cmd">
			./configure --prefix=/opt/openmpi <br>
			make <br>
			sudo make install <br>
		</div>
		<p> Cleaning </p>
		<div class="cmd">
			cd .. <br>
			rm -rf openmpi-4.0.1/ <br>
		</div>
		<p> Modify the /etc/bash.bashrc by adding the line: </p>
		<div class="notes">export PATH=/opt/openmpi/bin:$PATH</div>
		<p> Then source the file to take into consideration the modifications: </p>
		<div class="cmd">
			source /etc/bash.bashrc
		</div>
		<p> If the installation succeeds, you should use the mpicxx command in your terminal. Then proceed to the test of ECOGEN compilation in the previous <a href="{{ "/start" | prepend: site.baseurl }}"> page </a>. </p>
	</div>	


</article>

<!-- <article>
	<h2> Tutos </h2>
	<p> </p>
</article>

<article>
	<h2> User guide </h2>
	<p> </p>
</article> -->
