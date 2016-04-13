# Poster material

## Header
* Title, logos, names, etc
  - Katie prefers to use Kathleen
  - Should we include others (Razvan, Dr. Smith, Dr. Mattingly)?
  - Department logos?
    * Does the math department even have one? Doesn't look like it.
    * I think adding them will be cluttered anyhow and it's a pain.

## Left column

Left column will be focused on background material

* Explanation of source localization
  - Especially: difficulties
    * Modeling
    * Data requirements
    * Uncertainties
    * Expensive transport simulations
* Markov-Chain Monte Carlo
  - Relate to source localization
    * Explain in a Bayesian context
    * Why it is advantageous here
  - Different approaches
    * Outline Metropolis algorithm (make it look snazzy)
      - Can probably reuse that nicely typeset layout I made for M-H in the longer article
    * Other methods - DRAM, DREAM
  - (?) Discuss convergence
    * Might be too ambitious for a poster as this is a complicated topic
    * Maybe just "Convergence is hard in MCMC, take our word for it that we checked and are 
      pretty sure our chains are converged."
* ???

## Center Column

Middle column will focus on setup and the specific problem, plus how we address them.

* Transport model
  - Note simplifications:
    * 2D (pseudo-3D) ray-tracing
    * Stationary
    * Synthetic data [see below]
    * Uncollided flux
      - Justify this assumption in particular
    * Homogeneous geometry
      - Known XS, treat it as a volume homogenized mass
* Simulated geometry
  - Pretty picture! Enough said.
* (?) Discuss MCMC implementations in MATLAB and ~~DAKOTA~~ PyMC
  - Mention the DAKOTA results? Mehhhh.
* (?) Discuss generation of the synthetic data?
  - Cross sections?
    * I have MCNP geometry renderings that look pretty if we want to show how I simulated those
    * Can also include pretty plots of particle tracks in the slab if we have space
* ???

## Right column

Right column is results and conclusions.

* Posterior plots
  - Again, more pretty pictures!
    * Make sure to consistentify how my posteriors and Katie's are plotted (I can just replot her data?)
    * PyMC gives working intensities, so we can include plots for intensities if we have space.
* (?) Convergence plots
  - I have plots of G-R convergence metrics
    * Do we even want t
* Conclusions
  - Yep, we found it!
    * Different algorithms compare well
      - Make plots of speedups?
  - Need real data obviously
    * FIG
      - Can show a picture of the site and experiment plan if we have space.
    * MCNP
      - I have some preliminary results for this, they need to be refined a bit but so far things look
        really good. Errors in the cross section values seem to not have a whole lot of influence which
        is great because that's by far our biggest source of errors.
  - (?) Reduced source intensity
    * I've run this problem with a source that is an order of magnitude weaker and it worked fine, can mention if space
  - (???)
