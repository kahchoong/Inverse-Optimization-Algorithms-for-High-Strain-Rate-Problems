# Inverse problem to resolve high-strain rate plasticity behavior of materials from dynamic experimental data
![description](1-15.gif)

* The goal of my research, in general, is to understand inferrability of the plastic stress-strain curve from experimental data. Some experiments such as Taylor cylinder, Richtmeyer Meshkov Instabilities (RMI), Split Hopkinson Pressure Bar Test (SHPB) are commonly used already to directly measure the stress-strain response or dynamic strength. However, some metrics can be not quite so sensitive in resolving the stress-strain response (i.e. many different stress-strain responses can result from a similar enough experimental output) or very sensitive to small changes in parameters/error (ill-posedness). The work here has significance in understanding [planetary science](https://www.nature.com/articles/s41467-026-72210-4), [planetary defense](https://science.nasa.gov/mission/dart/), [materials under extreme conditions](https://pubmed.ncbi.nlm.nih.gov/38778107/), etc.
* What is an inverse problem?
* <b>What can we learn or takeaway?</b> There are many high-strain rate plasticity models out there that consider different types of dependencies (microstructure, deformation history etc.) and may only be useful for a given set of state variables (temperature, pressure, strain, strain rate). An optimizer can help us efficiently survey the parameter space and give us an idea of how a particular experimental output or model parameters may be sensitive (or too sensitive). This can, in turn, help build better models by truncating/adding certain terms or parameters, changing their relationships (logarithmic, linear, Arrhenius, etc.), or building a better experiment and collected output that responds more favorably.
* 
### Optimization algorithms considered so far (and am considering):
  * **[Nelder-Mead](https://en.wikipedia.org/wiki/Nelder%E2%80%93Mead_method)**
  * **[Covariance matrix adaptation evolution strategy (CMA-ES)](https://en.wikipedia.org/wiki/CMA-ES)**
  * **Bayesian Optimization**
  * **[Charged System Search (CSS)](https://link-springer-com.srv-proxy1.library.tamu.edu/article/10.1007/s00707-009-0270-4)**

### Important Topics/Focus Areas
 * Black-box or derivative-free optimization
 * Sensitivity & Error Analysis
 * Verification & Validation Problem (V&V)
 * Finite Element Method using Explicit Formulation/Hydrocodes
 * Dynamic Behavior of Materials & Shock Physics
 * 
### Workflow
Still thinking about ideas of how to organize the code and considering if I should make a PyPi package if there is enough interest and scalability/success with these algorithms

### References, Sources, Interesting Reads (at least sources that have made sense of what I am doing)
  1. Meyers, M. A. (1994). Dynamic behavior of materials. Wiley-Interscience. https://doi.org/10.1002/9780470172278
  2. [Visualizing the Nelder-Mead](https://alexdowad.github.io/visualizing-nelder-mead/)
  3. [Curse of dimensionality](https://en.wikipedia.org/wiki/Curse_of_dimensionality)
  4. [Basic Research Needs for Inverse Methods for Complex Systems under Uncertainty](https://www.osti.gov/biblio/2583339)
