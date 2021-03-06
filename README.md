# StatisticalInference

##graph help
http://t-redactyl.io/blog/2016/02/creating-plots-in-r-using-ggplot2-part-7-histograms.html
library(ggplot2)
library(grid)
library(gridExtra)
p1 = qplot(1:10, rnorm(10))
p2 = qplot(1:10, rnorm(10))
grid.arrange(p1, p2, ncol = 2, main = "Main title")

https://stackoverflow.com/questions/3541713/how-to-plot-two-histograms-together-in-r

http://www.sthda.com/english/wiki/ggplot2-title-main-axis-and-legend-titles

https://stackoverflow.com/questions/9360332/how-to-plot-density-plots-with-proportions-on-the-y-axis

## Kanh Academy CTL
https://www.khanacademy.org/math/statistics-probability/sampling-distributions-library/sample-means/v/central-limit-theorem
## Project Notes
https://www.youtube.com/watch?v=pTmLQvMM-1M&t=1s

read "Statistics for Dummies"

  Windows: MiKTeX (Complete) - http://miktex.org/2.9/setup
  (NOTE: Be sure to download the Complete rather than Basic installation)

###check list for project
https://github.com/lgreski/datasciencectacontent/blob/master/markdown/statinf-expDistChecklist.md

###Tips for tooth growth
https://github.com/lgreski/datasciencectacontent/blob/master/markdown/edaInToothGrowthAnalysis.md

remember to see the random variables

ased on the central limit theorem, the expected variance for the distribution of sample means is sigma^2 / N, not sigma^2. If we're taking samples of 40 exponentials, then N = 40. The expected standard deviation would be sigma / sqrt(N).

In your report, if you've created an array of 1000 means of 40 exponentials you can run pastecs::stat.desc() to obtain a variety of descriptive statistics on the array of means, including variance and standard deviation

The main thrust of the assignment is to compare the raw distribution of exponentials with the distribution of 1,000 means of 40 observations taken from an exponential distribution.




The Central Limit Theorem states that the distribution of means should be approximately normal (regardless of whether the underlying distribution is normal), with an expected value equal to the mean of the underlying distribution, and variance equal to the variance of the underlying distribution divided by the sample size.

The theoretical variance of an exponential distribution is 1 / lambda, not 1 / sqrt(n). Therefore, the expected variance of the distribution of sample means should be (1 / lambda) / (sample size), not 1 / sqrt(sample size).