# ProteinEvolver2
Modeling protein evolution forward in time accounting for simultaneous protein fitness

**ProteinEvolver2 README**




**Purpose**

ProteinEvolver models protein evolution forward in time under structure-based and empirical substitution models and considering evolutionary histories that can be: (1) obtained from the birth-death population process and based on the protein fitness of every variant at every time, (2) simulated with the coalescent under complex population models (recombination, migration, and demographics) or (3) user-specified as a phylogenetic tree. The file ProteinEvolver2_manual.pdf includes detailed documentation, and the user is strongly advised to read it carefully before using the program.

**Download and Installation**

Download the program from https://github.com/MiguelArenas/ProteinEvolver2. Open a console window. In the same directory as the file ProteinEvolver2.zip, type:

_unzip ProteinEvolver2.zip_

You should now see a folder called ProteinEvolver2. Note that this zip file was made on a Mac, so in Windows or Linux you might see some strange files, that start with "." or "-". These are Macintosh hidden files, which can be safely removed without affecting the software.

Executables for MacOSX and Linux Debian, are available inside the folder exe.

**Compilation**

The program should compile without problem in any Unix-like environment (Linux, MacOSX, etc.). A makefile is provided for the gcc compiler, but if you have cc instead, just change gcc for cc in the makefile. The default optimization level is set to -O3. To compile in Macintosh with an intel processor, and probably in the machines, you can enable the option -fast instead.

To compile the program move into the folder src inside the ProteinEvolver2 folder and type:

_make all_

Several warnings without importance could be shown on the screen depending on the used compilator, they can be ignored.

To clean the executable file (i.e., to compile again)

_make clean_

In the case of using the MPI version. The program should compile without problems with a second makefile "Makefile_MPI" for an MPI version. This makefile might need some modifications for a particular OS. To compile the program for MPI type:

_make -f Makefile_MPI_


**Execution**

The program runs in a command-line window. In MacOS X and Linux, the user needs to open the Terminal application, and in Windows XP the user should open the Command Prompt.

To run the program move to the folder where the executable is located and type:

_./ProteinEvolver2.1.1_

To execute the parallel version, MPI libraries have to be installed in the host. The minimum number of processors is two. An example of execution in 3 processors is the next:

_mpirun -np 3 ProteinEvolver2.1.1_

Arguments can be entered in the command line or, more conveniently, from a text file called "parameters" which should be located in the same directory as the executable. See the documentation for further details.


**Disclaimer**

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later 

version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA 02111-1307, USA.



**Credits and Funding**

Miguel Arenas - marenas@uvigo.es

2023

This work was supported by the Spanish Ministry of Economy and Competitiveness and the Ministry of Science and Innovation through the Grants RYC-2015-18241 and PID2019-107931GA-I00/AEI/10.13039/501100011033


