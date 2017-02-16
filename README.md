# Updating-a-Gaussian-Belief
This code demonstrates the superiority of Bayes' Statistics in online updating of beliefs. A 'Gaussian Bandit' is initiated, which produces samples from a normal distribution with 'unknown' parameters (they are set in the beginning by the user while initiating the bandit). An updating algorithm refines the estimated parameters and their respective distribution with the incoming data. A 3D plot of the resulting Normal-Inverse-Gamma Distribution is plotted (including contour plots) and a predict-function provides the probability of observing values within a specified range.
After copy, pasting, executing the code simply copy paste follwoing lines for a demonstration:


mean=2
sd=3
data=5
minlim=-3
maxlim=3

bandit1=gauss_bandit(mean,sd)
pull_and_update(bandit1,data)
bandit1.predict(minlim,maxlim)




The five values can be tweaked at will. The existing 'body of evidence' can be augmented with more information by simply running the pull_and_update function again with the same bandit and the desired amount of data.
