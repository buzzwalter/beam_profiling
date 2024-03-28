## Astigmatic Beam Profiling 
The $M^2$ value of a laser beam characterizes how a beam diverges from it's fundamental gaussian profile.  This is parameterized by the way it's longitudintal profile behaves via the equation

$$ \omega(z) = \omega_0 \sqrt{1 + M^4 (\frac{z}{z_R})^2}$$

where $\omega(z)$ is the transverse profile's radius at longitudinal distance $z$.

Ascertaining the $M^2$ value for beams is incredibly important in physics applications especially on the analysis side where the calculation of cross sections becomes important.  Companies will sell commercial beam profilers for thousands of dollars alongside expensive software that does what anyone with a relatively affordable USB camera and enough motivation to analyze data in ~~python~~ your  favorite high level language could do.  

The analysis centers around the calculation of the variance of the distrubution associated with the curve.  Curve fitting proves to be surperfluous when the beam is very non-gaussian, so it ends up being easier and more effective to use a monte carlo method.  For such a small task, computing power is of no concern.  

The most important this is the actual experimental procedure.  For this, the standard procedure to sample several points below half the Rayleigh length, 

$$z_R = \pi \omega_0^2 / \lambda,$$

and three quarters the rayleigh length. However increasing the total number of samples over the whole curve is still effective.  The reason for this methodology is choosing the appropriate beam parameters to collect quality data without having to move the camera too much is a priority and these regions typically allow for agreement between the various constraints.  
