<h1>About</h1>

This is a project submitted for a course in NTU, Singapore. The project uses current numerical methods to solve for th etrajectories of particles and simulates if these particles are detected at detectors which look for them.

To simulate the particle detectors, the decay of the particles are first simulated using the Metropolis-Hastings algorithm. With this, a target plate (which is a plate where the particles in consideration would decay from) decay simulation can be done, which looks like the image below

<p align="center">
  <img src="https://github.com/shsgResume/ParticlePhysicsDetectorSimulations/assets/167844966/6dfbd737-b3cc-48ca-b453-144eb4d75665" />
</p>
  
Depending on the decay probability the user inputs into the program, target plate may have more decays (red being decayed parts of the plate) or less. 

<p align="center">
  <img src="https://github.com/shsgResume/ParticlePhysicsDetectorSimulations/assets/167844966/d2b109c9-4fe4-4b8c-8e27-6783b0c33230" />
</p>

The decay would follow a Gaussian probability distribution, but the decay probability inputted by the user would be the cutoff. For example, the Gaussian distribution displays the decay of the target plate into anything, and 50% of the target plate would decay into anything on average. If the decay threshold to decay into a specific particle to consider, such as Kaons, would be at 40%, then only the parts above 60% of the Gaussian would be counted as a target plate decay into Kaons. 


After the probability of decaying has been computed, the probability where the particles will be detected at the detector comprises of its trajectory computations. The trajectory has noise built into it, but at the same time, magnetic horns can focus the particles to come in more refined bunches aimed towards the detectors.

For when there are no magnetic horns, the particles are seen to be more spread out

<p align="center">
  <img src="https://github.com/shsgResume/ParticlePhysicsDetectorSimulations/assets/167844966/74a3aa38-9aa1-4626-a791-44718f0e75ff" />
</p>

When there are horns, the particles are more bunched together

<p align="center">
  <img src="https://github.com/shsgResume/ParticlePhysicsDetectorSimulations/assets/167844966/81d63ce4-e92e-4b75-b4b5-becb47e87711" />
</p>

<h1>Requirements</h1>

> [!NOTE]
> Python<br>
> Numpy<br>
> Matplotlib<br>






