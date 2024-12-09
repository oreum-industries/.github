# Oreum Industries: Technical Resources

[Oreum Industries](https://oreum.io) is a data science consultancy from 
[Jonathan Sedar](https://github.com/jonsedar) in collaboration with a worldwide
network of expert developers and leaders. We focus on the insurance industry, 
helping underwriters, insurtechs and corporates to learn from data. We operate 
remotely & globally, with a client base spanning USA, UK, Europe and the Middle 
East.

Our technical bread and butter is advanced Bayesian statistical modeling, 
to create an edge in pricing & reserving throughout general & life insurance.
This is essential to quantify uncertainty and support underwriter-led real-world 
decision-making in low data environments.

As opportunity allows, we host a handful of technical resources here. In each 
case at least a Technical Overview is public, and in some cases we've made the 
code available to read, or even fully open-source. Naturally we can't open 
everything, so where code is closed, please contact 
[info@oreum.io](mailto:info@oreum.io) for commercial interest - we'd be more 
than happy to discuss in detail.

## Technical References

These are the result of a concise exploration and implementation of specific 
tools & techniques relevant to our modeling work. They often contain novel
model architectures, describe theory and practice at a deep level, and use 
Bayesian inference and a Bayesian workflow, specifically using the 
`pymc` & `arviz` ecosystem. 

+ [**Oreum Copula**](https://oreum-industries.github.io/oreum_copula/#/) 
  Copula Regression Modeling. This provides an extremely valuable method to 
  properly estimate Expected Loss Costs when Claims Frequency & Severity are 
  correlated in low data environments. _Public Intro Slides, Commercial License_.

+ [**Oreum Survival**](https://github.com/oreum-industries/oreum_survival) 
  Survival Regression Modeling. This provides an extremely valuable suite of 
  model architectures to estimate time-to-event via right-censored Accelerated 
  Failure Time (AFT) and semi-parametric (CoxPH) models. 
  _Publicly Readable Code, Commercial License_.

+ [**PYMC Examples: GLM-missing-values-in-covariates**](https://github.com/jonsedar/pymc-examples/blob/new-example-glm-ordinal-features/examples/generalized_linear_models/GLM-ordinal-features.ipynb). 
+ Full Bayesian workflow example on how to handle and impute missing data in 
  exogenous (predictor) covariates in `pymc`. 
  _Public Code, Open Source License, (pending PR)_.

+ [**PYMC Examples: GLM-ordinal-features**](https://github.com/jonsedar/pymc-examples/blob/new-example-glm-missing-numeric-values/examples/generalized_linear_models/GLM-missing-values-in-covariates.ipynb). 
+ Full Bayesian workflow example on how to handle ordinal data in exogenous 
  (predictor) covariates in `pymc`.
  _Public Code, Open Source License, (pending PR)_.


## Case Studies

These are the result of a deep-dive investigation into a particular dataset, 
either to learn about that data or to fully demonstrate a suite of methods to
tackle a new challenge.

+ [**Oreum Case Study: Lung**](https://oreum-industries.github.io/oreum_cs_lung/#/)
  Survival regression of a lung cancer mortality study with conventional 
  full-period observations. Uses a novel Accelerated Failure Time architecture 
  that handles right-censoring, missing data, ordinal covariates and a linear 
  regression submodel. _Public Overview Slides, Commercial License_.

+ [**Oreum Case Study: ONS**](https://oreum-industries.github.io/oreum_cs_ons/#/)
  Survival regression of a multi-year England & Wales ONS aggregated deaths-only 
  dataset. This is a very compromised dataset but interesting to tackle, and 
  requires a highly novel modified AFT architecture to allow for right-truncation 
  (not right-censoring). _Public Overview Slides, Commercial License_.
  
+ [**Oreum Wholelife Simulator**](https://github.com/oreum-industries/oreum_mre_wholelife)
   Simulate the cash value of WholeLife Insurance Policies using a parameterised
   survival curve including financial activities (investments, drawdowns).
  _Publicly Readable Code, Commercial License_.


## Support

These are supporting repos to aid high-quality software development on client 
projects

+ [**Oreum Core**](https://github.com/oreum-industries/oreum_core) Core tools
  used by Oreum Industries on client projects to make data science work faster,
  more repeatable and consistent etc. Includes various data diagnostics, EDA 
  plots, model factories, Bayesian model evaluation etc. 
  _Public Code, Open Source License_.

+ [**Oreum Template**](https://github.com/oreum-industries/oreum_template) A 
  reusable template project structure - all our projects adhere to this.
  _Publicly Readable Code, Commercial License_.


---
Oreum OÜ &copy; 2024
