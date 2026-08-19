# Inverse problem to resolve high-strain rate plasticity behavior of materials from dynamic experimental data
![description](1-15.gif)

* The goal of my research, in general, is to understand inferrability of the plastic stress-strain curve from experimental data. Some experiments such as Taylor cylinder, Richtmeyer Meshkov Instabilities (RMI), Split Hopkinson Pressure Bar Test (SHPB) are commonly used already to directly measure the stress-strain response or dynamic strength. However, some metrics can be not quite so sensitive in resolving the stress-strain response (i.e. many different stress-strain responses can result from a similar enough experimental output) or very sensitive to small changes in parameters/error (ill-posedness). The work here has significance in understanding [planetary science](https://www.nature.com/articles/s41467-026-72210-4), [planetary defense](https://science.nasa.gov/mission/dart/), [materials under extreme conditions](https://pubmed.ncbi.nlm.nih.gov/38778107/), etc.
* What is an inverse problem?
* <b>What can we learn or takeaway?</b> There are many high-strain rate plasticity models out there that consider different variables, may only be useful at a set of state variables, . An optimizer can help us gather evidence on if a particular experimental output or model parameters are sufficiently sensitive. Which can, in turn, help us build better models by truncating/adding certain terms or parameters, changing how they vary (logarithmic, exponential, linear, etc.), or developing a better experiment that responds more favorably.
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
 * Finite Element Method using Explicit Formulation
 * 
### Workflow
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; still thinking about ideas of how to organize the code and considering if I should make a PyPi package if there is enough interest and scalability/success with these algorithms

### References and Sources (at least the ones that have made sense of what I am doing)
  1. Meyers, M. A. (1994). Dynamic behavior of materials. Wiley-Interscience. https://doi.org/10.1002/9780470172278
  2. https://alexdowad.github.io/visualizing-nelder-mead/
  3. https://en.wikipedia.org/wiki/Curse_of_dimensionality
