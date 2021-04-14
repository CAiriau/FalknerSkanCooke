# FalknerSkanCooke
Solution of the Falkner-Skan Cooke equation in Fortran with a continuation method


## Sources

* The code is integrated into a Fortran module in the **src** directory

* For the compilation just write *make clean; make* in a terminal

* The executable named **fsc** will be located in a **~/bin** directory (eventually to create)


## Running

* The input file **fsc_continuation.in** is in the **run** directory.

* To get the solution write **fsc** in a terminal or **./x1.run.sh**

* The bash script **x1.run.sh** can clean your directory, run the code or compile it.


## Validation

* Results with Falkner-Skan solutions have been valided for a long time.

* Additional results with the Cooke equations have been validated directly with the Cooke (1950) results.


## Methodology

* Two integration schemes are available : 4th Runge-Kutta (RK4) and explicit ordrer 1 Euler (EEO1)
* For RK4 the normal step size can be at least of order 0.01
* For EEO1, it is adviced to choose a very small step size, lower than 0.001, 0.001 is better
* A Newton algorithm is implemented to solve first FSK equations, and then (optional) Cooke equation
* The boundary layer thickness is a part of the convergence algorithm, the user does not have to set it precisely. 


## Documentation

* A documention has been generated with *Doxygen*.

* Open the **index.html** file in the **doc/build/html** directory

* To generate the documentation use the script **./x1.Doxygen**


## History

Please read the doc.


## Version

* Version 2. 
* The code is derived from the FSK code including in my **FundAeroSuite** deposit

C.A.  April 2021

