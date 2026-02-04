# STATS 67 Introduction to Probability and Statistics for CS

## R

### Basic functions
- function structure
do(somthing)
- form a table
data.frame()
- get help
?()


### Summarizing data
- Count
count(dataset, variable)
- Mean
summarize(dataset, mean(variable))
- Median
summarize(dataset, media(vairable))
- Quantile (eg. Q3)
summarize(dataset, quantile(variable, 0.75))
- Standard Deviation
summarize(dataset, sd(variable))
- Variance
summarize(dataset, var(variable))

### Plots
- Bar plots
ggplot(dataset, aes(x = variable)) + geom_bar()
- Histogram
ggplot(dataset, aes(x = variable)) + geom_histogram()
- Boxplot
ggplot(dataset, aes(x = variableX, y = variableY)) + geom_boxplot()
- Scatterplot
ggplot(dataset, aes(x = variableX, y = variableY, color = variableZ)) + geom_point()

### Simple random sampling
sample(x = 1:N, size = n, replace = FALSE)


### Distribution
#### Discrete distributions
##### Bernoulli distributions
##### Geometric distributions
- pmf: dgeom(x, prob)
- cdf: pgeom(q, prob)

##### Binomial distributions
- pmf: dbinom(x, size, prob)
- cdf: pbinom(q, size, prob)

##### Poisson distribution
- pmf: dpois(x, lambda)
- cdf: ppois(x, lambda)

#### Continuous distributions
##### Exponential distribution
- cdf: pexp(q, rate)

##### Normal Distribution
- cdf: pnorm(q, mean, sd)
- cdf: pnorm(q, mean, sd, lower.tail = FALSE)
- INVERSEcdf: qnorm(p, mean, sd)

##### Continuous uniform distribution
- pdf: dunif(x, min, max)
- cdf: punif(x, min, max)