This is an adaptation made by: 

	Alex D. Santos Sosa 
	Univeristy of Puerto Rico, Rio Piedras Campus
	Department of Computer Science
	801-11-7707 


==================================================================================
 This file is part of BCCD, an open-source live CD for computational science
 education.
 
 Copyright (C) 2010 Andrew Fitz Gibbon, Paul Gray, Kevin Hunter, Dave Joiner, 
   Sam Leeman-Munk, Tom Murphy, Charlie Peck, Skylar Thompson, & Aaron Weeden 
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
==================================================================================

Area-Under The Curve:
This is an adaptation of the Area-Under the Curve program provided by BCCD. In this program instead of calculating the area under the curve of the function x^2 we calculate the area under the curve of e^(-x). 

Included are a Makefile that produces area.c-serial and area.c-mpi-openmp using area.c. area.c-serial finds the area serialy and area.c-mpi-openmp finds the area using nodes and threads.
 
How to Build:
  $ make 

How To Run:
  To run a program (e.g. hybrid) with a domain from 0.0 to 10.0 and with 
  100000000 rectangles, use: qsub area.hybrid.qsub

  To run a program (e.g. serial) with the default left x-boundary of the
  domain and 10.0 as the right x-boundary of the domain with 
  100000000 rectangles, use: qsub area.serial.qsub

Credit Aaron Weeden for this explanation.
