## Data input

Put  defined dataPara.mat file as below into the 'input' folder

​	$S$ $-$ the total number of vessels.

​	$P$  $-$ the total number of stockpiles.

​	$K$  $-$ the total number of berths.

​	$R$  $-$ the total number of reclaimers.

​	$U$  $-$ the total number of reclaiming lines.

​	$V$  $-$ the total number of conveyor lines.

​	$W$  $-$ the total number of ship loading lines.

​	$C$  $-$ the total number of types.

​	$M$  $-$ the total number of tasks.

​	$T$  $-$ time interval to optimize.

​	$Para.Pset$  $-$ set of stockpiles.

​	$Para.Uset$  $-$ set of reclaiming lines.

​	$Para.Vset$  $-$ set of conveyor lines.

​	$Para.Wset$  $-$ set of ship loading lines.

​	$Para.Rset$  $-$ set of reclaimers.

​	$Para.Kset$  $-$ set of berths.

​	${Para.{Dm}}$ $--$ The dry bulk quantity required for task $m$.

​	${Para.{Cm}}$ $--$ The dry bulk type required for task $m$.

​	$Para.{deltaMK}$ $--$ Accessibility between ship-loading task $m$ and berth $k$.

​	${Para.betaSK}$ $--$ Vessel $s$ docks at berth $k$.

​	${ Para.thetaSM}$ $--$ Vessel $s$ executes task $m$.

​	$ Para.SMset $ $--$ Set of tasks executed by vessels.

​	${ Para.gammaMP}$ $--$ Accessibility between ship-loading task $m$ and stockpile position $p$.

​	${Para.lambdaUR}$ $--$ Accessibility between reclaiming line $u$ and reclaimer $r$.

​	${Para.lambdaURset}$ $--$ Set of reclaimers available on each reclaiming line.

 	$Para.alphaUP$ $--$ Accessibility between reclaiming line $u$ and stockpile position $p$. 

​	$alphaUPset$ $--$ Set of stockpiles available on each reclaiming line.

​	$Para.alphaWK$ $--$ Accessibility between ship loading line $w$ and berth $k$.

​	$Para.alphaWKset$ $--$ Set of ship loading lines for each berth.

 	$ Para.alphaUVW$ $--$ Accessibility among reclaiming line $u$, conveyor line $v$ and ship loading line $w$.

​	${Para.Krr}$ $--$ Reclaimers $r$ and ${r}'$ are on the same reclaiming line.

​	$ Para.DtPK $ $--$ The material transportation time from reclaiming stockpile $p$ to berth $k$, where the vessel is located.

​	$ Para.Vr$ $--$ Operational efficiency of reclaimer $r$.

​	$ {Para.t\_arr}$ $--$ Arrival time at port of vessel $s$.

​	$ Para.t\_tr $ $--$ Turnaround time of vessel $s$.

​	$ Para.t\_un$ $--$ Casting-off time of vessel $s$.

​	$ Para.t\_aux$ $--$ Auxiliary operation time of vessel $s$.

​	$ Para.paiKK$ $--$ Travel time for shiploader from berth $k$ to ${k}'$.

# 2. Execute the 'KMA.exe'

​	The GUI interface displays program execution progress and final results: running time and best solution.


# 3. Data Output

​	The KMAtrend.mat will saved in the 'output' file.

​	

# 4. KMA Executable

1. Prerequisites for Deployment 

Verify that version 9.10 (R2021a) of the MATLAB Runtime is installed.   
If not, you can run the MATLAB Runtime installer.
To find its location, enter

    >>mcrinstaller

at the MATLAB prompt.
NOTE: You will need administrator rights to run the MATLAB Runtime installer. 

Alternatively, download and install the Windows version of the MATLAB Runtime for R2021a 
from the following link on the MathWorks website:

    https://www.mathworks.com/products/compiler/mcr/index.html

For more information about the MATLAB Runtime and the MATLAB Runtime installer, see 
"Distribute Applications" in the MATLAB Compiler documentation  
in the MathWorks Documentation Center.

2. Files to Deploy and Package

Files to Package for Standalone 

-KMA.exe
-MCRInstaller.exe 
    Note: if end users are unable to download the MATLAB Runtime using the
    instructions in the previous section, include it when building your 
    component by clicking the "Runtime included in package" link in the
    Deployment Tool.
-This readme file 



3. Definitions

For information on deployment terminology, go to
https://www.mathworks.com/help and select MATLAB Compiler >
Getting Started > About Application Deployment >
Deployment Product Terms in the MathWorks Documentation
Center.
