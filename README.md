# LBeyondGR (vs.0.1) package for Mathematica
A simple-to-use Mathematica package to (i) ray trace null geodesics in stationary, axisymmetric, and asymptotically flat spacetimes, (ii) numerically bisect potentially non-star-convex lensing-band boundaries, and (iii) minimize the overlap of the resulting geometric lensing band with respect to an observational prior.

The LBeyondGR package currently incorporates:

- Numerical ray tracing in arbitrary stationary and axisymmetric spacetimes. The only restriction is that the spacetime be expressed in terms of coordinates which converge to oblate spheroidal coordinates at asymptotically large values of the radial coordinate.

- Free-floating lensing-band bisections (see also App.~A of the accompanying publication 2311.xxxxx).

- The use of Mathematica's "Geometric Computation" capabilities and specifically NMinimize[] to minimize the overlap of an observed/assumed lensed emission region and the obtained lensing band.

This is not an official release and the authors cannot exclude bugs. Both, the numerical efficiency and accuracy largely rely on Mathematica's internal NDSolve[] and NMinimize[] routines. The code is far from optimized.
For current efforts to port the capabilities to a (more) runtime optimized and python-based code, please contact the author.

# Author & Contact
If you have any questions on this project, please contact 
Aaron Held
(held.aaron@gmail.com)

# Acknowledgement
If your research is based on or benefits from this package or the associated conceptual lensing-band framework, please consider citing
A. Held, A. Cárdenas-Avendaño, 2311.xxxxx.

# Installation

Simply clone the full directory and call the package via
	Import["../pkg/LBeyondGR.m"]
as in the example .nb's in /examples.

# Dependencies

The current version has been tested on Mathematica 12.
For now, the user has to make sure to import the spacetime metric and associated Christoffel symbols in an appropriate format. An automatic determination of the Christoffel symbols requires the xAct package and is not yet implemented in the public version. In case you are interested, please contact the author. 

# How to use
Example files explain the usage of the package.
Once the package is loaded, the usual ?Function command in Mathematica packages provides minimal information on how to use a function. The author apologizes for not finding time for more complete documentation and hopes to improve the documentation in future releases.
If you are planning to use the package for your work and have any questions, please do not hesitate to contact the author.
